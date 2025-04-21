## [1.2.0](https://github.com/Knighten-Homelab/gha-reusable-workflows/compare/1.1.4...1.2.0) (2025-04-21)

### Features

* created gha to launch awx job template ([741d877](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/741d877ea6e9ce36761d8082c4554b8e24f9365a))

## [1.1.4](https://github.com/Knighten-Homelab/gha-reusable-workflows/compare/1.1.3...1.1.4) (2025-04-21)

### Bug Fixes

* moved end-to-end deployment ghas to use new awx playbook gha ([eb5c661](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/eb5c661c8a4065209776ac24b06a2280926a5f98))

## [1.1.3](https://github.com/Knighten-Homelab/gha-reusable-workflows/compare/1.1.2...1.1.3) (2025-04-20)

### Bug Fixes

* made awx_project_branch equal to run ref ([cb79b92](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/cb79b9274ec66a61d3dfedfb515700871dd43228))

## [1.1.2](https://github.com/Knighten-Homelab/gha-reusable-workflows/compare/1.1.1...1.1.2) (2025-04-20)

### Bug Fixes

* moved from pipx to pip for awx resource playbook gha ([fc7572c](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/fc7572c8b496ce602e315d7c524ceef13e409754))

## [1.1.1](https://github.com/Knighten-Homelab/gha-reusable-workflows/compare/1.1.0...1.1.1) (2025-04-20)

### Bug Fixes

* removed default dir in awx playback gha ([52b4b62](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/52b4b6209569e31515164f6d7b07c2e8254fd81b))

## [1.1.0](https://github.com/Knighten-Homelab/gha-reusable-workflows/compare/1.0.0...1.1.0) (2025-04-20)

### Features

* created gha to deploy an awx resource based playbook ([89bc917](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/89bc917728c54317af20867a1e3fb16983c245b4))

## [1.0.0](https://github.com/Knighten-Homelab/gha-reusable-workflows/compare/...1.0.0) (2025-04-17)

### Bug Fixes

* added names to jobs ([f17f032](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/f17f0321129c42f158c9b75b3875d433157fe8e1))
* added node js install before tf actions ([330836f](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/330836f182e406ae57be58f4797bae42df8faa8f))
* added node to tf lint gha ([dc86052](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/dc860528e525764d7a655af70a0b7786d6ba8043))
* added pdns api key as tf var for apply ([5a6c937](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/5a6c937e2c2dee613737f2e524dbb07063d57430))
* cleaned up trivy output ([15f8bbd](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/15f8bbdda0a2df5940cc4964497269c475d2e6af))
* correct initial tab level ([d8da5a9](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/d8da5a978934db16e90a067cb7a6fd38a185dd70))
* corrected job name for semantic-release ([71b1f77](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/71b1f77f4dc411695279e6d720853eba160da241))
* corrected version used for semantic release ([ac61d5f](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/ac61d5fcb09c164ea0b6f434c514c0228b34a947))
* introduced ansible-dir var to tf ghas and renamed script var to playbook ([f3e0b23](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/f3e0b23694abdaa9e8c978beb5a2e84b2e198b59))
* removed _TEST from vault secrets in destroy ([7dec22a](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/7dec22a1e24317dfc2596a83699638c1f0fd3203))
* removed required on run-on input ([2cbddb1](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/2cbddb1a2a6381b47f90e566fdeb8f5a8fb1e58e))
* removed trailing / ([89c8679](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/89c867960cd5309a6c0056e10feb817a179a3773))
* renamed semantic-release to semantic-release-to-gh.yaml ([57c119d](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/57c119daebec332d150499302d163f71863afde1))
* updated semantic-release depends versions ([89b183e](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/89b183ea14d22ce737dd9fd5cc5aed6ce257880b))

### Features

* added a runs-on var for semantic-release ([aa7cc9e](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/aa7cc9e87f48154443e4a9b4a543bca749566570))
* added gha to ansible code ([777de52](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/777de5237e221bdf63b6867634442995696398f3))
* added gha to apply tf and deploy app via awx ([9074a48](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/9074a48701ac73314a6ac1348f5bdc4a4d2d25b8))
* added gha to get repos latest tag ([eb63a41](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/eb63a41d7bed90236886a68eb176696156b76842))
* added git ref variable to all ghas that defaults to the runs ref ([cff00d2](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/cff00d23ac70e598200d0632313c705eecc84015))
* added README content ([aaf20e2](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/aaf20e26cb44d5cf223e564570ceba9e2544bbfb))
* added release gha ([994caa4](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/994caa4070aa18bf9ddfa88098afd882c55b67d0))
* added semantic release gha ([4fa5370](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/4fa5370b2be57f07ceb9d79e9b22e2ca1098745f))
* added terraform lint and scan gha ([e5328b7](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/e5328b7bf266859e938eb13ee84bc83aee9ca53d))
* made gha to undeploy app ([2c473c9](https://github.com/Knighten-Homelab/gha-reusable-workflows/commit/2c473c92a2d6c425f27e3840b569f0e8738366c5))
