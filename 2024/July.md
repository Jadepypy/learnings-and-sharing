Goal for the second sprint as it's already mid-July:
Summer is my favorite season and I think this the best time of the year!
"Study hard in the most undisciplined, irreverent, and original manner possible." - keep in mind!

* First thing first, finish draft SOP (painful, seemingly a waste of time but in fact a good practice for self-reflection and future planning.
* CKA exam prep, exam date is in August
  * outlines (to be added, try better than pasting syllabus directly from Udemy)
  * skills
    * vim
    * kubectl with kalias and Bash autocompletion 
    * jq for YAML/JSON processing 
    * tmux for terminal multiplexing 
    * curl and wget for testing web services
* Yunikorn (Kubernetes scheduler) contribution
  * tasks 
  * learning outlines (to be added)

7/15
* SOP draft done

7/16
* why is pod the smallest unit in Kubernetes?
  * Containers can be seemed as single process; Pod can be seen as a group of containers that share the same network namespace...
    * though multiple processes are allowed in a container, but it does not have the convention of having a init process as pid 1 which may be tricky when handling) 
  * Kubernetes design pattern: pod is can be seen as simple as an atomic unit of abstraction, which is designed for the convenience of developers (ex: do not need to consider the network design for each container in the pod but for pod itself only)
* the controllers for Kubernetes, a reconciliation loop that checks if the controlled object is in the desired state
  * a controller like Deployment can normally be split into two parts: expected state, controlled object template (ex: Pod template)
  * should be closely related to the declarative apis in Kubernetes
* no hands on experiment today zzz


TODO: 
* [Design Patterns for Container-based Distributed Systems](https://www.usenix.org/conference/hotcloud16/workshop-program/presentation/burns) 