# Changelog

## [2.4.0](https://github.com/celestecaprine/zonaite/compare/v2.3.0...v2.4.0) (2023-06-03)


### Features

* added Helix ([143d711](https://github.com/celestecaprine/zonaite/commit/143d711b8e909da7c98db2684f0f598d2776293c))
* added silverbrew-server ([92d604e](https://github.com/celestecaprine/zonaite/commit/92d604e2bbaea0e41a61502ce0773afec2741e2f))
* rename project to zonaite ([eb02f0a](https://github.com/celestecaprine/zonaite/commit/eb02f0ac364be304f1f309ff2d80d63995aef29d))


### Bug Fixes

* change version to a working version for recipe-serv ([a5b6e3b](https://github.com/celestecaprine/zonaite/commit/a5b6e3b5eecaa4f54506c3fe3e7f607dc84b54ef))

## 2.3.0 (2023-06-01)


### ⚠ BREAKING CHANGES

* optimize container layers and reduce image size
* only deploy the branch named "live", to simplify development
* remove legacy PWA setup command from custom.just
* move justfile to standardized, non-conflicting new location
* add new recipe flag which allows you to completely disable yafti
* enhanced autostart.desktop to use new script, and always find icon
* move all autostart-related files to standardized location
* move firstboot reference to new yafti.yml location ([#72](https://github.com/celestecaprine/silverbrew/issues/72))
* move yafti.yml to standardized location
* move justfile to standardized location
* move recipe.yml to standardized location
* change base-container to base-image ([#49](https://github.com/celestecaprine/silverbrew/issues/49))

### Features

* add a just setup command for setting up nix ([#48](https://github.com/celestecaprine/silverbrew/issues/48)) ([1d208f6](https://github.com/celestecaprine/silverbrew/commit/1d208f6eaec5000daab9e4bce69e5547a916df89))
* add back usr folder ([9f47c1e](https://github.com/celestecaprine/silverbrew/commit/9f47c1eddfc00779de2fc4c07bb6816bda9adf76))
* add boot_menu.yml ([46de2ed](https://github.com/celestecaprine/silverbrew/commit/46de2edecc56f0bcf8dc231e0ede7a44408330e6))
* Add code-of-conduct ([#39](https://github.com/celestecaprine/silverbrew/issues/39)) ([aab8078](https://github.com/celestecaprine/silverbrew/commit/aab8078cfdc7d2354e057a0ca4771d3a53d2df4c))
* add conventional commit linting and release notes generator ([b7820b4](https://github.com/celestecaprine/silverbrew/commit/b7820b4ba312ca939d0dc977ed9f6a08d135324b))
* add cosign.key to gitignore ([#51](https://github.com/celestecaprine/silverbrew/issues/51)) ([5f4ac04](https://github.com/celestecaprine/silverbrew/commit/5f4ac049a7f60bb55e40da809e29ac1dd9f65fc9))
* add extra repos field to recipe ([#52](https://github.com/celestecaprine/silverbrew/issues/52)) ([c537104](https://github.com/celestecaprine/silverbrew/commit/c537104ba2695a3c843ba7e67e7a118665f50c9a))
* add fedora 38 build ([#45](https://github.com/celestecaprine/silverbrew/issues/45)) ([69fd4d7](https://github.com/celestecaprine/silverbrew/commit/69fd4d7a57c5ce39331e47e8dedeb2a2f643190f))
* add function for reading individual YAML strings ([33ab88f](https://github.com/celestecaprine/silverbrew/commit/33ab88f7940b6e360d3e8d7f4a1b0b393547dd92))
* add how to review a PR ([#76](https://github.com/celestecaprine/silverbrew/issues/76)) ([ae2e25b](https://github.com/celestecaprine/silverbrew/commit/ae2e25b92f5ebebed2fcaad53ecfab651a639d12))
* add new recipe flag which allows you to completely disable yafti ([32c06b0](https://github.com/celestecaprine/silverbrew/commit/32c06b0867b0e4f66c3d1dfa303530682c16a52f))
* add per-recipe shell script support ([#38](https://github.com/celestecaprine/silverbrew/issues/38)) ([37143b0](https://github.com/celestecaprine/silverbrew/commit/37143b0e23582f8754808b77aee4b594bb877ba1))
* add virt-manager and libvirt ([5d03718](https://github.com/celestecaprine/silverbrew/commit/5d03718e19559f4b93c7254dd20a919f7f9e4b0f))
* add yafti.yml from bluefin ([f9a1561](https://github.com/celestecaprine/silverbrew/commit/f9a1561f2c8a718890f4d932db8ce625342610e2))
* automatic repo version selection via YAML configuration ([baa8c47](https://github.com/celestecaprine/silverbrew/commit/baa8c47ffa97ae25077d205432bec0c549b27319))
* change description for more information ([33ddd2b](https://github.com/celestecaprine/silverbrew/commit/33ddd2bbac6eebbf4716af0465808f2e2fe56ebc))
* declare base image and fedora ver in recipe ([fe16187](https://github.com/celestecaprine/silverbrew/commit/fe16187a92400865b4f96e82ce4d6781478bdfe6))
* declare image description in recipe.yml ([c9c011d](https://github.com/celestecaprine/silverbrew/commit/c9c011d842a9ef9ec5d3976a0fd167b22ca0f0ed))
* declare image name in recipe.yml ([2b40d4b](https://github.com/celestecaprine/silverbrew/commit/2b40d4b4367c669f1e557194db7bc14ac40f8b53))
* ease customization by reading flatpaks and rpms to install from a recipe.yml. ([#79](https://github.com/celestecaprine/silverbrew/issues/79)) ([a5e90a5](https://github.com/celestecaprine/silverbrew/commit/a5e90a588f58a938405bf513d1032955be34028e))
* enable manually running build ([2521741](https://github.com/celestecaprine/silverbrew/commit/2521741049e25b13c3865225be26c3d63aa84a21))
* gha for building / publishing on pr ([#87](https://github.com/celestecaprine/silverbrew/issues/87)) ([1726d18](https://github.com/celestecaprine/silverbrew/commit/1726d182ee95ce5eb13f47212799a68b63c5aefc))
* implement a very flexible runner for "pre" and "post" scripts ([55ff636](https://github.com/celestecaprine/silverbrew/commit/55ff6363be7a783a5949ede05575d2936a4c6e29))
* implement effortless RPM removal via YAML configuration ([bf19fa5](https://github.com/celestecaprine/silverbrew/commit/bf19fa5eca5b6440f4cfe83aa33c2c2e5797d33e))
* include flowchart graphic which explains new launcher hierarchy ([2f85593](https://github.com/celestecaprine/silverbrew/commit/2f85593176abfe9eafdd59780d7909e386af4c15))
* install repos first, so that they're available for scripting ([d09dd76](https://github.com/celestecaprine/silverbrew/commit/d09dd7624355076616735f82e066f364c0d02470))
* Install VanillaOS' first-setup ([#55](https://github.com/celestecaprine/silverbrew/issues/55)) ([43ddf0a](https://github.com/celestecaprine/silverbrew/commit/43ddf0a123911f9dedc3a76dcfc314a7cb37e871))
* leave a warning for people to move to new repo ([#99](https://github.com/celestecaprine/silverbrew/issues/99)) ([ffcb397](https://github.com/celestecaprine/silverbrew/commit/ffcb3973bd540d679ab033ed94de6336b903e7dd))
* new "autostart" binary, for easy startup customization ([8a5fd31](https://github.com/celestecaprine/silverbrew/commit/8a5fd31f8877ff425dd360ab2cd8a63e67ddd95a))
* only deploy the branch named "live", to simplify development ([da17603](https://github.com/celestecaprine/silverbrew/commit/da17603567bd7206a844d932c1cac34329d05817))
* refactor build.sh to use the new yafti launcher ([63a5e35](https://github.com/celestecaprine/silverbrew/commit/63a5e3583b1f3fdd4224e5f7cf9844c7a2b3f0da))
* sanity check Flathub's existence on all systems and all users ([aa157c2](https://github.com/celestecaprine/silverbrew/commit/aa157c2514f8725e7535501fc4a02f95544a5850))
* split flatpak update units into user and system ([#72](https://github.com/celestecaprine/silverbrew/issues/72)) ([99c15be](https://github.com/celestecaprine/silverbrew/commit/99c15be6f012cb590891c5ef16b2613dc538d144))
* streamlined YAML configuration for RPM-related settings ([4ca33a3](https://github.com/celestecaprine/silverbrew/commit/4ca33a3fe37afeb14a5e764813f623be7c2af042))
* swap out custom build for RPM of vanilla-first-setup ([#59](https://github.com/celestecaprine/silverbrew/issues/59)) ([6927892](https://github.com/celestecaprine/silverbrew/commit/6927892581dadf8f31419a0d9b070bb7268513ba))
* switch to separate build script ([68122c8](https://github.com/celestecaprine/silverbrew/commit/68122c87cacbadc47bd85403c2d1c5b5b49eab3f))
* switch to yafti for first boot ([0b669f5](https://github.com/celestecaprine/silverbrew/commit/0b669f5bb502c5e334474c54c95fbb7fed184b36))
* tag PR builds independently from matrix.version, latest, and stable ([b022183](https://github.com/celestecaprine/silverbrew/commit/b02218386235e6d40a11a48b5b1171e9acf8d1eb))
* ultimate laziness achieved with a powerful new script runner ([5cacb2f](https://github.com/celestecaprine/silverbrew/commit/5cacb2fcd86aa499aba4188ef6357e7e008373bc))
* update artifacthub readme url ([6cc44ff](https://github.com/celestecaprine/silverbrew/commit/6cc44ff4a9462727260733d9c973aae5a3f90c46))
* use a recipe matrix ([1bfabe6](https://github.com/celestecaprine/silverbrew/commit/1bfabe674e92dd5bf7fc12956941857de4eacd0a))
* use Fedora 38 ([#64](https://github.com/celestecaprine/silverbrew/issues/64)) ([60ddd67](https://github.com/celestecaprine/silverbrew/commit/60ddd67713b1fd843377276dbefb1afd54e23cc0))
* yafti package group for recipe.yml ([0cf6b13](https://github.com/celestecaprine/silverbrew/commit/0cf6b13b6c44135848ae9a400b2fa3aa5aed657d))


### Bug Fixes

* $IMAGE_NAME -&gt; ${{ env.IMAGE_NAME }} ([678ab12](https://github.com/celestecaprine/silverbrew/commit/678ab12c5ac41751775ca6898d09e2d09ea2d8b3))
* add a warning that we change the flatpak configuration ([#80](https://github.com/celestecaprine/silverbrew/issues/80)) ([9a349e2](https://github.com/celestecaprine/silverbrew/commit/9a349e2625791b90c11f640938060344ec3e4bd5))
* add flags to ensure that build aborts if there are errors ([4b9fe0b](https://github.com/celestecaprine/silverbrew/commit/4b9fe0b05bd138cebd825e67cb6c5a062181d6d8))
* add libadwaita ([#45](https://github.com/celestecaprine/silverbrew/issues/45)) ([ec91345](https://github.com/celestecaprine/silverbrew/commit/ec91345bc71b373b3fa5aff4ad3df0eefec45fa4))
* add path for boot_menu.yml ([8c520d0](https://github.com/celestecaprine/silverbrew/commit/8c520d0a3481f9338bc335d2ce72b0abc38f9c77))
* add pip for yafti, remove zenity (unneeded) ([9e827fe](https://github.com/celestecaprine/silverbrew/commit/9e827fe6be1495221cecc83746d266a78c55ba96))
* add recipe build arg ([#23](https://github.com/celestecaprine/silverbrew/issues/23)) ([a27e3cf](https://github.com/celestecaprine/silverbrew/commit/a27e3cfa13fbf76e145a6fcd4bb469d42daf5995))
* add shebang ([97ee716](https://github.com/celestecaprine/silverbrew/commit/97ee7169f4a287520b516bc377b90046b717daaf))
* add the missing GNOME Core apps to "yafti" template ([7c3ae59](https://github.com/celestecaprine/silverbrew/commit/7c3ae599e521fdab197dd8710f3b38b057d3f007))
* Add vte dependency for first-setup ([#56](https://github.com/celestecaprine/silverbrew/issues/56)) ([f8917a3](https://github.com/celestecaprine/silverbrew/commit/f8917a3258196f85b8e3805f5ebcb1c9c0db06a7))
* add zenity to not break if th FROM is changed ([9b3578b](https://github.com/celestecaprine/silverbrew/commit/9b3578b2175d4ad2427736ff7a7e3bc962ea35f0))
* allow forks to push to registry with label ([#86](https://github.com/celestecaprine/silverbrew/issues/86)) ([14b1b7c](https://github.com/celestecaprine/silverbrew/commit/14b1b7cb044ec616817aa30075609469dcb9986b))
* artifact upload/extract ([#88](https://github.com/celestecaprine/silverbrew/issues/88)) ([6590066](https://github.com/celestecaprine/silverbrew/commit/6590066ebcf72d6c4a56730dd682088db17d7df0))
* automatically determine current fedora version during build ([946f3d8](https://github.com/celestecaprine/silverbrew/commit/946f3d82eec8bfb12a187c00b31aa5ac512fa0d7))
* change boot menu to match available images ([04a754f](https://github.com/celestecaprine/silverbrew/commit/04a754f7e5b508032483d1e181740ffd27f3f60c))
* change img to startingpoint in verification ([21eafaa](https://github.com/celestecaprine/silverbrew/commit/21eafaa3c09c888f8b90a0345855a5024a24dacb))
* chore: manual merge action updates from main  ([#41](https://github.com/celestecaprine/silverbrew/issues/41)) ([a9c15ac](https://github.com/celestecaprine/silverbrew/commit/a9c15ac30655689f15e83e2534335f2b49a4622b))
* corrected readme ([9d831ac](https://github.com/celestecaprine/silverbrew/commit/9d831ac736a658ae9949e17363abacfb37618f2b))
* declare image name in one place ([73de53c](https://github.com/celestecaprine/silverbrew/commit/73de53cd39fbc4a5c84e27d9df7215f91d689ab4))
* don't copy usr as it's empty ([8b389d5](https://github.com/celestecaprine/silverbrew/commit/8b389d5f049c6e9c74c9a742edf798d52beaab28))
* Don't generate an image when README.md is updated ([#36](https://github.com/celestecaprine/silverbrew/issues/36)) ([8c170cf](https://github.com/celestecaprine/silverbrew/commit/8c170cfe89dd306eec0940f4dc50ed245c94bc2b))
* enhanced autostart.desktop to use new script, and always find icon ([ec4d01c](https://github.com/celestecaprine/silverbrew/commit/ec4d01caa8dfeeb152e474a40d7485903be98edd))
* extremely robust handling for YAML data fetching ([07cbe2c](https://github.com/celestecaprine/silverbrew/commit/07cbe2cc08908ffef4a4543f2e50f0c3a80ed559))
* faster installation of custom RPMs ([5f072b8](https://github.com/celestecaprine/silverbrew/commit/5f072b8b671ccb68b8e15aff62abebda4ac1115a))
* friendlier experience in the "yafti" first boot template ([c7deb7d](https://github.com/celestecaprine/silverbrew/commit/c7deb7d6fe3aa4256d7a79123ffc250a24165263))
* further improve portability of login-profile.sh ([4318180](https://github.com/celestecaprine/silverbrew/commit/4318180a7c134fc06c83bac550c90c50678550d8))
* improve "yq" arguments in justfile ([abbb283](https://github.com/celestecaprine/silverbrew/commit/abbb283dbe69d1e126a8bf41141c517cdda0d488))
* loop over lines, functional var substitution ([773fc23](https://github.com/celestecaprine/silverbrew/commit/773fc23804d7f6d5c044d46c28564a62d709f171))
* move all autostart-related files to standardized location ([34f6189](https://github.com/celestecaprine/silverbrew/commit/34f6189d26043b0efb4242d186cfc211a0a16c14))
* move firstboot reference to new yafti.yml location ([#72](https://github.com/celestecaprine/silverbrew/issues/72)) ([7004136](https://github.com/celestecaprine/silverbrew/commit/700413653ee904c20a5ba2eb365dcfda33c77fec))
* move justfile to standardized location ([07642c2](https://github.com/celestecaprine/silverbrew/commit/07642c2f43167d13b51ef3b29fa0679908fa8d93))
* move justfile to standardized, non-conflicting new location ([cec7397](https://github.com/celestecaprine/silverbrew/commit/cec73978cf2ff49b0aad5278485e8854f5738519))
* move recipe.yml to standardized location ([077e724](https://github.com/celestecaprine/silverbrew/commit/077e7243f264840cb71b801335cc9b728ee73813))
* move yafti.yml to standardized location ([8ee9967](https://github.com/celestecaprine/silverbrew/commit/8ee996722f698d585651b252d60ef57d59fc1627))
* moving recipe back to a directory available on the host ([#47](https://github.com/celestecaprine/silverbrew/issues/47)) ([95ff830](https://github.com/celestecaprine/silverbrew/commit/95ff830b49649fd3d76f54e7cce1727ace6ac6c6))
* only create yafti grp when flatpaks defined ([#46](https://github.com/celestecaprine/silverbrew/issues/46)) ([b3f7f07](https://github.com/celestecaprine/silverbrew/commit/b3f7f07d6ceca0489d699c6d2dfa4d995588c5c1))
* only generate date tag for main branch ([94aa5bb](https://github.com/celestecaprine/silverbrew/commit/94aa5bb8df2aac0985d4c9422b19b0c03a3f25b0))
* optimize container layers and reduce image size ([e8b5be6](https://github.com/celestecaprine/silverbrew/commit/e8b5be6e83099043a4aa51460154940af3ee7ce2))
* pre-generate empty "pre" and "post" script directories ([f0946f7](https://github.com/celestecaprine/silverbrew/commit/f0946f74b9c93c46a57186d7df6d9310c1fb508b))
* prevent /etc/ merge issues ([#43](https://github.com/celestecaprine/silverbrew/issues/43)) ([085d26a](https://github.com/celestecaprine/silverbrew/commit/085d26aa1acd7252c1c54fbd18661fed1a69d4e1))
* re-tag image ([#92](https://github.com/celestecaprine/silverbrew/issues/92)) ([a831ce0](https://github.com/celestecaprine/silverbrew/commit/a831ce00df84d94e2bdb48013f650bcbb5b39568))
* remove -y flag from yq; not in  go version ([5a98ef6](https://github.com/celestecaprine/silverbrew/commit/5a98ef653293d5d3a9b4f0920d3625291a93601a))
* remove 38 ([#89](https://github.com/celestecaprine/silverbrew/issues/89)) ([8a6f343](https://github.com/celestecaprine/silverbrew/commit/8a6f3433ad45b0f9f3da974a691001c02f498fb1))
* remove 38 builds and fix logo metadata ([#62](https://github.com/celestecaprine/silverbrew/issues/62)) ([521f0ad](https://github.com/celestecaprine/silverbrew/commit/521f0adcda598a1bf494d969df375f0c0a03a10c))
* remove akmods script as it's redundant ([c3b6c1a](https://github.com/celestecaprine/silverbrew/commit/c3b6c1af83ab6d41f531d7f990927087ad60b09f))
* remove duplicate flatpaks from recipe.yml ([4afc5b1](https://github.com/celestecaprine/silverbrew/commit/4afc5b1b4482ec6eb5e1841cbb57d3d9e3d98f5c))
* remove extremely verbose "x" flag ([20e0a06](https://github.com/celestecaprine/silverbrew/commit/20e0a06588e9b0e4edb3522f4d9602d2e681f4af))
* remove if statements ([#96](https://github.com/celestecaprine/silverbrew/issues/96)) ([0c7bc17](https://github.com/celestecaprine/silverbrew/commit/0c7bc17666ae038a0504d24a0e683f724c734527))
* remove legacy PWA setup command from custom.just ([ecb6fde](https://github.com/celestecaprine/silverbrew/commit/ecb6fdebb17240de5a80c8cf9e54d99623f0dab6))
* remove old pr workflow sections ([#98](https://github.com/celestecaprine/silverbrew/issues/98)) ([4a21580](https://github.com/celestecaprine/silverbrew/commit/4a21580f4e4d40692449bae61a75a555e8569be1))
* remove RPMs after installing RPMs, to guarantee cleanup ([3920ba9](https://github.com/celestecaprine/silverbrew/commit/3920ba9ab53fd75e5b54fdecdd330e0a80fcc0bb))
* remove unneeded escape ([616c59c](https://github.com/celestecaprine/silverbrew/commit/616c59c90bebd1d4dda24d5c28fa35adb067b13a))
* rename package back to `base` ([#97](https://github.com/celestecaprine/silverbrew/issues/97)) ([785b8f0](https://github.com/celestecaprine/silverbrew/commit/785b8f0d8adb8513bbe94b8918bfc0033ee0ca45))
* restore download artifact step, support multi-line tags ([#90](https://github.com/celestecaprine/silverbrew/issues/90)) ([c40bddf](https://github.com/celestecaprine/silverbrew/commit/c40bddfdf39a61545700ecb8123a02abd24a4f8f))
* retain variables ([091e939](https://github.com/celestecaprine/silverbrew/commit/091e9396f2929bee6a3cf1606439377f75f13a92))
* revert previous commit ([5947af4](https://github.com/celestecaprine/silverbrew/commit/5947af45da9ea324ab8c52e09142c916791d88e2))
* switch profile.d script to more robust technique ([c4b6b47](https://github.com/celestecaprine/silverbrew/commit/c4b6b4760606c9f70c30a88c9b20474e5698cc95))
* thoroughly remove fedora Flatpaks, and install unfiltered Flathub ([475a3c9](https://github.com/celestecaprine/silverbrew/commit/475a3c91cdfced27b73ad80a6d5e1ec19617d932))
* typo in /usr ([bd5db68](https://github.com/celestecaprine/silverbrew/commit/bd5db68387150ee04afc348bfdfd42afdc4db167))
* typo in workflow_dispatch ([fbd14f5](https://github.com/celestecaprine/silverbrew/commit/fbd14f502f6c2ceaeb02f6b7ddab246b7a507171))
* update cosign action ([#94](https://github.com/celestecaprine/silverbrew/issues/94)) ([0aff9ba](https://github.com/celestecaprine/silverbrew/commit/0aff9bac374c3494f57a360fd4426afe705bfee9))
* update cosign installer version ([#32](https://github.com/celestecaprine/silverbrew/issues/32)) ([91d4c38](https://github.com/celestecaprine/silverbrew/commit/91d4c3877ca61595f4e1f6a5cfa5dbf4dcc0e596))
* use default boot_menu.yml for testing purposes ([486d2fa](https://github.com/celestecaprine/silverbrew/commit/486d2fa9ab7231b51949bee27bd1b720ca89414f))
* use proper shebang line ([f24c407](https://github.com/celestecaprine/silverbrew/commit/f24c4072fdb09f117f8e2b58baf017883725b7a0))
* use RECIPE arg ([6d77885](https://github.com/celestecaprine/silverbrew/commit/6d778859c82924e920198c69c2e27bbabdf3ea3e))
* use yq in setup-flatpaks ([66d2265](https://github.com/celestecaprine/silverbrew/commit/66d22650f02cb4c551675614168b44eb89cb8345))


### Styles

* change base-container to base-image ([#49](https://github.com/celestecaprine/silverbrew/issues/49)) ([1df862a](https://github.com/celestecaprine/silverbrew/commit/1df862aae8472f765828043d0ae1bea2953b61a0))


### Miscellaneous Chores

* release 2.3.0 ([600520f](https://github.com/celestecaprine/silverbrew/commit/600520fc74fa73ba88009700958578d17a015477))

## [2.1.3](https://github.com/celestecaprine/silverbrew/compare/v2.1.2...v2.1.3) (2023-05-31)


### Bug Fixes

* change boot menu to match available images ([1fc919b](https://github.com/celestecaprine/silverbrew/commit/1fc919bf1e9156d442f3f0546c0e0c67ad795d12))

## [2.1.2](https://github.com/celestecaprine/silverbrew/compare/v2.1.1...v2.1.2) (2023-05-31)


### Bug Fixes

* add path for boot_menu.yml ([6e94f60](https://github.com/celestecaprine/silverbrew/commit/6e94f6069b973f0793e5093f7b7b6c6bb624a4a2))

## [2.1.1](https://github.com/celestecaprine/silverbrew/compare/v2.1.0...v2.1.1) (2023-05-31)


### Bug Fixes

* use default boot_menu.yml for testing purposes ([4aff1b2](https://github.com/celestecaprine/silverbrew/commit/4aff1b211c14f1d1dd0daba096735ffdb5e040aa))

## [2.1.0](https://github.com/celestecaprine/silverbrew/compare/v2.0.0...v2.1.0) (2023-05-31)


### Features

* add boot_menu.yml ([659f8a9](https://github.com/celestecaprine/silverbrew/commit/659f8a9c18a66b5718533972d18a8e0bc00aff33))

## [2.0.0](https://github.com/celestecaprine/silverbrew/compare/v1.0.0...v2.0.0) (2023-05-31)


### ⚠ BREAKING CHANGES

* remove kmod-wl from kmods to install

### Bug Fixes

* remove kmod-wl from kmods to install ([28ed0ee](https://github.com/celestecaprine/silverbrew/commit/28ed0eef6eb3f0b7aac8b179f48ed164c77cab41))

## 1.0.0 (2023-05-30)


### ⚠ BREAKING CHANGES

* optimize container layers and reduce image size
* only deploy the branch named "live", to simplify development
* remove legacy PWA setup command from custom.just
* move justfile to standardized, non-conflicting new location
* add new recipe flag which allows you to completely disable yafti
* enhanced autostart.desktop to use new script, and always find icon
* move all autostart-related files to standardized location
* move firstboot reference to new yafti.yml location ([#72](https://github.com/celestecaprine/silverbrew/issues/72))
* move yafti.yml to standardized location
* move justfile to standardized location
* move recipe.yml to standardized location
* change base-container to base-image ([#49](https://github.com/celestecaprine/silverbrew/issues/49))

### Features

* add a just setup command for setting up nix ([#48](https://github.com/celestecaprine/silverbrew/issues/48)) ([1d208f6](https://github.com/celestecaprine/silverbrew/commit/1d208f6eaec5000daab9e4bce69e5547a916df89))
* add back usr folder ([9f47c1e](https://github.com/celestecaprine/silverbrew/commit/9f47c1eddfc00779de2fc4c07bb6816bda9adf76))
* Add code-of-conduct ([#39](https://github.com/celestecaprine/silverbrew/issues/39)) ([aab8078](https://github.com/celestecaprine/silverbrew/commit/aab8078cfdc7d2354e057a0ca4771d3a53d2df4c))
* add conventional commit linting and release notes generator ([b7820b4](https://github.com/celestecaprine/silverbrew/commit/b7820b4ba312ca939d0dc977ed9f6a08d135324b))
* add cosign.key to gitignore ([#51](https://github.com/celestecaprine/silverbrew/issues/51)) ([5f4ac04](https://github.com/celestecaprine/silverbrew/commit/5f4ac049a7f60bb55e40da809e29ac1dd9f65fc9))
* add extra repos field to recipe ([#52](https://github.com/celestecaprine/silverbrew/issues/52)) ([c537104](https://github.com/celestecaprine/silverbrew/commit/c537104ba2695a3c843ba7e67e7a118665f50c9a))
* add fedora 38 build ([#45](https://github.com/celestecaprine/silverbrew/issues/45)) ([69fd4d7](https://github.com/celestecaprine/silverbrew/commit/69fd4d7a57c5ce39331e47e8dedeb2a2f643190f))
* add function for reading individual YAML strings ([33ab88f](https://github.com/celestecaprine/silverbrew/commit/33ab88f7940b6e360d3e8d7f4a1b0b393547dd92))
* add how to review a PR ([#76](https://github.com/celestecaprine/silverbrew/issues/76)) ([ae2e25b](https://github.com/celestecaprine/silverbrew/commit/ae2e25b92f5ebebed2fcaad53ecfab651a639d12))
* add new recipe flag which allows you to completely disable yafti ([32c06b0](https://github.com/celestecaprine/silverbrew/commit/32c06b0867b0e4f66c3d1dfa303530682c16a52f))
* add per-recipe shell script support ([#38](https://github.com/celestecaprine/silverbrew/issues/38)) ([37143b0](https://github.com/celestecaprine/silverbrew/commit/37143b0e23582f8754808b77aee4b594bb877ba1))
* add yafti.yml from bluefin ([f9a1561](https://github.com/celestecaprine/silverbrew/commit/f9a1561f2c8a718890f4d932db8ce625342610e2))
* automatic repo version selection via YAML configuration ([baa8c47](https://github.com/celestecaprine/silverbrew/commit/baa8c47ffa97ae25077d205432bec0c549b27319))
* change description for more information ([33ddd2b](https://github.com/celestecaprine/silverbrew/commit/33ddd2bbac6eebbf4716af0465808f2e2fe56ebc))
* declare base image and fedora ver in recipe ([fe16187](https://github.com/celestecaprine/silverbrew/commit/fe16187a92400865b4f96e82ce4d6781478bdfe6))
* declare image description in recipe.yml ([c9c011d](https://github.com/celestecaprine/silverbrew/commit/c9c011d842a9ef9ec5d3976a0fd167b22ca0f0ed))
* declare image name in recipe.yml ([2b40d4b](https://github.com/celestecaprine/silverbrew/commit/2b40d4b4367c669f1e557194db7bc14ac40f8b53))
* ease customization by reading flatpaks and rpms to install from a recipe.yml. ([#79](https://github.com/celestecaprine/silverbrew/issues/79)) ([a5e90a5](https://github.com/celestecaprine/silverbrew/commit/a5e90a588f58a938405bf513d1032955be34028e))
* enable manually running build ([2521741](https://github.com/celestecaprine/silverbrew/commit/2521741049e25b13c3865225be26c3d63aa84a21))
* gha for building / publishing on pr ([#87](https://github.com/celestecaprine/silverbrew/issues/87)) ([1726d18](https://github.com/celestecaprine/silverbrew/commit/1726d182ee95ce5eb13f47212799a68b63c5aefc))
* implement a very flexible runner for "pre" and "post" scripts ([55ff636](https://github.com/celestecaprine/silverbrew/commit/55ff6363be7a783a5949ede05575d2936a4c6e29))
* implement effortless RPM removal via YAML configuration ([bf19fa5](https://github.com/celestecaprine/silverbrew/commit/bf19fa5eca5b6440f4cfe83aa33c2c2e5797d33e))
* include flowchart graphic which explains new launcher hierarchy ([2f85593](https://github.com/celestecaprine/silverbrew/commit/2f85593176abfe9eafdd59780d7909e386af4c15))
* install repos first, so that they're available for scripting ([d09dd76](https://github.com/celestecaprine/silverbrew/commit/d09dd7624355076616735f82e066f364c0d02470))
* Install VanillaOS' first-setup ([#55](https://github.com/celestecaprine/silverbrew/issues/55)) ([43ddf0a](https://github.com/celestecaprine/silverbrew/commit/43ddf0a123911f9dedc3a76dcfc314a7cb37e871))
* leave a warning for people to move to new repo ([#99](https://github.com/celestecaprine/silverbrew/issues/99)) ([ffcb397](https://github.com/celestecaprine/silverbrew/commit/ffcb3973bd540d679ab033ed94de6336b903e7dd))
* new "autostart" binary, for easy startup customization ([8a5fd31](https://github.com/celestecaprine/silverbrew/commit/8a5fd31f8877ff425dd360ab2cd8a63e67ddd95a))
* only deploy the branch named "live", to simplify development ([da17603](https://github.com/celestecaprine/silverbrew/commit/da17603567bd7206a844d932c1cac34329d05817))
* refactor build.sh to use the new yafti launcher ([63a5e35](https://github.com/celestecaprine/silverbrew/commit/63a5e3583b1f3fdd4224e5f7cf9844c7a2b3f0da))
* sanity check Flathub's existence on all systems and all users ([aa157c2](https://github.com/celestecaprine/silverbrew/commit/aa157c2514f8725e7535501fc4a02f95544a5850))
* split flatpak update units into user and system ([#72](https://github.com/celestecaprine/silverbrew/issues/72)) ([99c15be](https://github.com/celestecaprine/silverbrew/commit/99c15be6f012cb590891c5ef16b2613dc538d144))
* streamlined YAML configuration for RPM-related settings ([4ca33a3](https://github.com/celestecaprine/silverbrew/commit/4ca33a3fe37afeb14a5e764813f623be7c2af042))
* swap out custom build for RPM of vanilla-first-setup ([#59](https://github.com/celestecaprine/silverbrew/issues/59)) ([6927892](https://github.com/celestecaprine/silverbrew/commit/6927892581dadf8f31419a0d9b070bb7268513ba))
* switch to separate build script ([68122c8](https://github.com/celestecaprine/silverbrew/commit/68122c87cacbadc47bd85403c2d1c5b5b49eab3f))
* switch to yafti for first boot ([0b669f5](https://github.com/celestecaprine/silverbrew/commit/0b669f5bb502c5e334474c54c95fbb7fed184b36))
* tag PR builds independently from matrix.version, latest, and stable ([b022183](https://github.com/celestecaprine/silverbrew/commit/b02218386235e6d40a11a48b5b1171e9acf8d1eb))
* ultimate laziness achieved with a powerful new script runner ([5cacb2f](https://github.com/celestecaprine/silverbrew/commit/5cacb2fcd86aa499aba4188ef6357e7e008373bc))
* update artifacthub readme url ([6cc44ff](https://github.com/celestecaprine/silverbrew/commit/6cc44ff4a9462727260733d9c973aae5a3f90c46))
* use a recipe matrix ([1bfabe6](https://github.com/celestecaprine/silverbrew/commit/1bfabe674e92dd5bf7fc12956941857de4eacd0a))
* use Fedora 38 ([#64](https://github.com/celestecaprine/silverbrew/issues/64)) ([60ddd67](https://github.com/celestecaprine/silverbrew/commit/60ddd67713b1fd843377276dbefb1afd54e23cc0))
* yafti package group for recipe.yml ([0cf6b13](https://github.com/celestecaprine/silverbrew/commit/0cf6b13b6c44135848ae9a400b2fa3aa5aed657d))


### Bug Fixes

* $IMAGE_NAME -&gt; ${{ env.IMAGE_NAME }} ([678ab12](https://github.com/celestecaprine/silverbrew/commit/678ab12c5ac41751775ca6898d09e2d09ea2d8b3))
* add a warning that we change the flatpak configuration ([#80](https://github.com/celestecaprine/silverbrew/issues/80)) ([9a349e2](https://github.com/celestecaprine/silverbrew/commit/9a349e2625791b90c11f640938060344ec3e4bd5))
* add flags to ensure that build aborts if there are errors ([4b9fe0b](https://github.com/celestecaprine/silverbrew/commit/4b9fe0b05bd138cebd825e67cb6c5a062181d6d8))
* add libadwaita ([#45](https://github.com/celestecaprine/silverbrew/issues/45)) ([ec91345](https://github.com/celestecaprine/silverbrew/commit/ec91345bc71b373b3fa5aff4ad3df0eefec45fa4))
* add pip for yafti, remove zenity (unneeded) ([9e827fe](https://github.com/celestecaprine/silverbrew/commit/9e827fe6be1495221cecc83746d266a78c55ba96))
* add recipe build arg ([#23](https://github.com/celestecaprine/silverbrew/issues/23)) ([a27e3cf](https://github.com/celestecaprine/silverbrew/commit/a27e3cfa13fbf76e145a6fcd4bb469d42daf5995))
* add shebang ([97ee716](https://github.com/celestecaprine/silverbrew/commit/97ee7169f4a287520b516bc377b90046b717daaf))
* add the missing GNOME Core apps to "yafti" template ([7c3ae59](https://github.com/celestecaprine/silverbrew/commit/7c3ae599e521fdab197dd8710f3b38b057d3f007))
* Add vte dependency for first-setup ([#56](https://github.com/celestecaprine/silverbrew/issues/56)) ([f8917a3](https://github.com/celestecaprine/silverbrew/commit/f8917a3258196f85b8e3805f5ebcb1c9c0db06a7))
* add zenity to not break if th FROM is changed ([9b3578b](https://github.com/celestecaprine/silverbrew/commit/9b3578b2175d4ad2427736ff7a7e3bc962ea35f0))
* allow forks to push to registry with label ([#86](https://github.com/celestecaprine/silverbrew/issues/86)) ([14b1b7c](https://github.com/celestecaprine/silverbrew/commit/14b1b7cb044ec616817aa30075609469dcb9986b))
* artifact upload/extract ([#88](https://github.com/celestecaprine/silverbrew/issues/88)) ([6590066](https://github.com/celestecaprine/silverbrew/commit/6590066ebcf72d6c4a56730dd682088db17d7df0))
* automatically determine current fedora version during build ([946f3d8](https://github.com/celestecaprine/silverbrew/commit/946f3d82eec8bfb12a187c00b31aa5ac512fa0d7))
* change img to startingpoint in verification ([21eafaa](https://github.com/celestecaprine/silverbrew/commit/21eafaa3c09c888f8b90a0345855a5024a24dacb))
* chore: manual merge action updates from main  ([#41](https://github.com/celestecaprine/silverbrew/issues/41)) ([a9c15ac](https://github.com/celestecaprine/silverbrew/commit/a9c15ac30655689f15e83e2534335f2b49a4622b))
* corrected readme ([9d831ac](https://github.com/celestecaprine/silverbrew/commit/9d831ac736a658ae9949e17363abacfb37618f2b))
* declare image name in one place ([73de53c](https://github.com/celestecaprine/silverbrew/commit/73de53cd39fbc4a5c84e27d9df7215f91d689ab4))
* don't copy usr as it's empty ([8b389d5](https://github.com/celestecaprine/silverbrew/commit/8b389d5f049c6e9c74c9a742edf798d52beaab28))
* Don't generate an image when README.md is updated ([#36](https://github.com/celestecaprine/silverbrew/issues/36)) ([8c170cf](https://github.com/celestecaprine/silverbrew/commit/8c170cfe89dd306eec0940f4dc50ed245c94bc2b))
* enhanced autostart.desktop to use new script, and always find icon ([ec4d01c](https://github.com/celestecaprine/silverbrew/commit/ec4d01caa8dfeeb152e474a40d7485903be98edd))
* extremely robust handling for YAML data fetching ([07cbe2c](https://github.com/celestecaprine/silverbrew/commit/07cbe2cc08908ffef4a4543f2e50f0c3a80ed559))
* faster installation of custom RPMs ([5f072b8](https://github.com/celestecaprine/silverbrew/commit/5f072b8b671ccb68b8e15aff62abebda4ac1115a))
* friendlier experience in the "yafti" first boot template ([c7deb7d](https://github.com/celestecaprine/silverbrew/commit/c7deb7d6fe3aa4256d7a79123ffc250a24165263))
* further improve portability of login-profile.sh ([4318180](https://github.com/celestecaprine/silverbrew/commit/4318180a7c134fc06c83bac550c90c50678550d8))
* improve "yq" arguments in justfile ([abbb283](https://github.com/celestecaprine/silverbrew/commit/abbb283dbe69d1e126a8bf41141c517cdda0d488))
* loop over lines, functional var substitution ([773fc23](https://github.com/celestecaprine/silverbrew/commit/773fc23804d7f6d5c044d46c28564a62d709f171))
* move all autostart-related files to standardized location ([34f6189](https://github.com/celestecaprine/silverbrew/commit/34f6189d26043b0efb4242d186cfc211a0a16c14))
* move firstboot reference to new yafti.yml location ([#72](https://github.com/celestecaprine/silverbrew/issues/72)) ([7004136](https://github.com/celestecaprine/silverbrew/commit/700413653ee904c20a5ba2eb365dcfda33c77fec))
* move justfile to standardized location ([07642c2](https://github.com/celestecaprine/silverbrew/commit/07642c2f43167d13b51ef3b29fa0679908fa8d93))
* move justfile to standardized, non-conflicting new location ([cec7397](https://github.com/celestecaprine/silverbrew/commit/cec73978cf2ff49b0aad5278485e8854f5738519))
* move recipe.yml to standardized location ([077e724](https://github.com/celestecaprine/silverbrew/commit/077e7243f264840cb71b801335cc9b728ee73813))
* move yafti.yml to standardized location ([8ee9967](https://github.com/celestecaprine/silverbrew/commit/8ee996722f698d585651b252d60ef57d59fc1627))
* moving recipe back to a directory available on the host ([#47](https://github.com/celestecaprine/silverbrew/issues/47)) ([95ff830](https://github.com/celestecaprine/silverbrew/commit/95ff830b49649fd3d76f54e7cce1727ace6ac6c6))
* only create yafti grp when flatpaks defined ([#46](https://github.com/celestecaprine/silverbrew/issues/46)) ([b3f7f07](https://github.com/celestecaprine/silverbrew/commit/b3f7f07d6ceca0489d699c6d2dfa4d995588c5c1))
* only generate date tag for main branch ([94aa5bb](https://github.com/celestecaprine/silverbrew/commit/94aa5bb8df2aac0985d4c9422b19b0c03a3f25b0))
* optimize container layers and reduce image size ([e8b5be6](https://github.com/celestecaprine/silverbrew/commit/e8b5be6e83099043a4aa51460154940af3ee7ce2))
* pre-generate empty "pre" and "post" script directories ([f0946f7](https://github.com/celestecaprine/silverbrew/commit/f0946f74b9c93c46a57186d7df6d9310c1fb508b))
* prevent /etc/ merge issues ([#43](https://github.com/celestecaprine/silverbrew/issues/43)) ([085d26a](https://github.com/celestecaprine/silverbrew/commit/085d26aa1acd7252c1c54fbd18661fed1a69d4e1))
* re-tag image ([#92](https://github.com/celestecaprine/silverbrew/issues/92)) ([a831ce0](https://github.com/celestecaprine/silverbrew/commit/a831ce00df84d94e2bdb48013f650bcbb5b39568))
* remove -y flag from yq; not in  go version ([5a98ef6](https://github.com/celestecaprine/silverbrew/commit/5a98ef653293d5d3a9b4f0920d3625291a93601a))
* remove 38 ([#89](https://github.com/celestecaprine/silverbrew/issues/89)) ([8a6f343](https://github.com/celestecaprine/silverbrew/commit/8a6f3433ad45b0f9f3da974a691001c02f498fb1))
* remove 38 builds and fix logo metadata ([#62](https://github.com/celestecaprine/silverbrew/issues/62)) ([521f0ad](https://github.com/celestecaprine/silverbrew/commit/521f0adcda598a1bf494d969df375f0c0a03a10c))
* remove duplicate flatpaks from recipe.yml ([4afc5b1](https://github.com/celestecaprine/silverbrew/commit/4afc5b1b4482ec6eb5e1841cbb57d3d9e3d98f5c))
* remove extremely verbose "x" flag ([20e0a06](https://github.com/celestecaprine/silverbrew/commit/20e0a06588e9b0e4edb3522f4d9602d2e681f4af))
* remove if statements ([#96](https://github.com/celestecaprine/silverbrew/issues/96)) ([0c7bc17](https://github.com/celestecaprine/silverbrew/commit/0c7bc17666ae038a0504d24a0e683f724c734527))
* remove legacy PWA setup command from custom.just ([ecb6fde](https://github.com/celestecaprine/silverbrew/commit/ecb6fdebb17240de5a80c8cf9e54d99623f0dab6))
* remove old pr workflow sections ([#98](https://github.com/celestecaprine/silverbrew/issues/98)) ([4a21580](https://github.com/celestecaprine/silverbrew/commit/4a21580f4e4d40692449bae61a75a555e8569be1))
* remove RPMs after installing RPMs, to guarantee cleanup ([3920ba9](https://github.com/celestecaprine/silverbrew/commit/3920ba9ab53fd75e5b54fdecdd330e0a80fcc0bb))
* remove unneeded escape ([616c59c](https://github.com/celestecaprine/silverbrew/commit/616c59c90bebd1d4dda24d5c28fa35adb067b13a))
* rename package back to `base` ([#97](https://github.com/celestecaprine/silverbrew/issues/97)) ([785b8f0](https://github.com/celestecaprine/silverbrew/commit/785b8f0d8adb8513bbe94b8918bfc0033ee0ca45))
* restore download artifact step, support multi-line tags ([#90](https://github.com/celestecaprine/silverbrew/issues/90)) ([c40bddf](https://github.com/celestecaprine/silverbrew/commit/c40bddfdf39a61545700ecb8123a02abd24a4f8f))
* retain variables ([091e939](https://github.com/celestecaprine/silverbrew/commit/091e9396f2929bee6a3cf1606439377f75f13a92))
* revert previous commit ([5947af4](https://github.com/celestecaprine/silverbrew/commit/5947af45da9ea324ab8c52e09142c916791d88e2))
* switch profile.d script to more robust technique ([c4b6b47](https://github.com/celestecaprine/silverbrew/commit/c4b6b4760606c9f70c30a88c9b20474e5698cc95))
* thoroughly remove fedora Flatpaks, and install unfiltered Flathub ([475a3c9](https://github.com/celestecaprine/silverbrew/commit/475a3c91cdfced27b73ad80a6d5e1ec19617d932))
* typo in /usr ([bd5db68](https://github.com/celestecaprine/silverbrew/commit/bd5db68387150ee04afc348bfdfd42afdc4db167))
* typo in workflow_dispatch ([fbd14f5](https://github.com/celestecaprine/silverbrew/commit/fbd14f502f6c2ceaeb02f6b7ddab246b7a507171))
* update cosign action ([#94](https://github.com/celestecaprine/silverbrew/issues/94)) ([0aff9ba](https://github.com/celestecaprine/silverbrew/commit/0aff9bac374c3494f57a360fd4426afe705bfee9))
* update cosign installer version ([#32](https://github.com/celestecaprine/silverbrew/issues/32)) ([91d4c38](https://github.com/celestecaprine/silverbrew/commit/91d4c3877ca61595f4e1f6a5cfa5dbf4dcc0e596))
* use proper shebang line ([f24c407](https://github.com/celestecaprine/silverbrew/commit/f24c4072fdb09f117f8e2b58baf017883725b7a0))
* use RECIPE arg ([6d77885](https://github.com/celestecaprine/silverbrew/commit/6d778859c82924e920198c69c2e27bbabdf3ea3e))
* use yq in setup-flatpaks ([66d2265](https://github.com/celestecaprine/silverbrew/commit/66d22650f02cb4c551675614168b44eb89cb8345))


### Styles

* change base-container to base-image ([#49](https://github.com/celestecaprine/silverbrew/issues/49)) ([1df862a](https://github.com/celestecaprine/silverbrew/commit/1df862aae8472f765828043d0ae1bea2953b61a0))

## [1.1.0](https://github.com/ublue-os/base/compare/v1.0.0...v1.1.0) (2023-03-03)


### Features

* add fedora 38 build ([#45](https://github.com/ublue-os/base/issues/45)) ([69fd4d7](https://github.com/ublue-os/base/commit/69fd4d7a57c5ce39331e47e8dedeb2a2f643190f))
* add how to review a PR ([#76](https://github.com/ublue-os/base/issues/76)) ([ae2e25b](https://github.com/ublue-os/base/commit/ae2e25b92f5ebebed2fcaad53ecfab651a639d12))
* ease customization by reading flatpaks and rpms to install from a recipe.yml. ([#79](https://github.com/ublue-os/base/issues/79)) ([a5e90a5](https://github.com/ublue-os/base/commit/a5e90a588f58a938405bf513d1032955be34028e))
* gha for building / publishing on pr ([#87](https://github.com/ublue-os/base/issues/87)) ([1726d18](https://github.com/ublue-os/base/commit/1726d182ee95ce5eb13f47212799a68b63c5aefc))
* Install VanillaOS' first-setup ([#55](https://github.com/ublue-os/base/issues/55)) ([43ddf0a](https://github.com/ublue-os/base/commit/43ddf0a123911f9dedc3a76dcfc314a7cb37e871))
* leave a warning for people to move to new repo ([#99](https://github.com/ublue-os/base/issues/99)) ([ffcb397](https://github.com/ublue-os/base/commit/ffcb3973bd540d679ab033ed94de6336b903e7dd))
* split flatpak update units into user and system ([#72](https://github.com/ublue-os/base/issues/72)) ([99c15be](https://github.com/ublue-os/base/commit/99c15be6f012cb590891c5ef16b2613dc538d144))
* swap out custom build for RPM of vanilla-first-setup ([#59](https://github.com/ublue-os/base/issues/59)) ([6927892](https://github.com/ublue-os/base/commit/6927892581dadf8f31419a0d9b070bb7268513ba))


### Bug Fixes

* add a warning that we change the flatpak configuration ([#80](https://github.com/ublue-os/base/issues/80)) ([9a349e2](https://github.com/ublue-os/base/commit/9a349e2625791b90c11f640938060344ec3e4bd5))
* Add vte dependency for first-setup ([#56](https://github.com/ublue-os/base/issues/56)) ([f8917a3](https://github.com/ublue-os/base/commit/f8917a3258196f85b8e3805f5ebcb1c9c0db06a7))
* allow forks to push to registry with label ([#86](https://github.com/ublue-os/base/issues/86)) ([14b1b7c](https://github.com/ublue-os/base/commit/14b1b7cb044ec616817aa30075609469dcb9986b))
* artifact upload/extract ([#88](https://github.com/ublue-os/base/issues/88)) ([6590066](https://github.com/ublue-os/base/commit/6590066ebcf72d6c4a56730dd682088db17d7df0))
* re-tag image ([#92](https://github.com/ublue-os/base/issues/92)) ([a831ce0](https://github.com/ublue-os/base/commit/a831ce00df84d94e2bdb48013f650bcbb5b39568))
* remove 38 ([#89](https://github.com/ublue-os/base/issues/89)) ([8a6f343](https://github.com/ublue-os/base/commit/8a6f3433ad45b0f9f3da974a691001c02f498fb1))
* remove 38 builds and fix logo metadata ([#62](https://github.com/ublue-os/base/issues/62)) ([521f0ad](https://github.com/ublue-os/base/commit/521f0adcda598a1bf494d969df375f0c0a03a10c))
* remove if statements ([#96](https://github.com/ublue-os/base/issues/96)) ([0c7bc17](https://github.com/ublue-os/base/commit/0c7bc17666ae038a0504d24a0e683f724c734527))
* remove old pr workflow sections ([#98](https://github.com/ublue-os/base/issues/98)) ([4a21580](https://github.com/ublue-os/base/commit/4a21580f4e4d40692449bae61a75a555e8569be1))
* rename package back to `base` ([#97](https://github.com/ublue-os/base/issues/97)) ([785b8f0](https://github.com/ublue-os/base/commit/785b8f0d8adb8513bbe94b8918bfc0033ee0ca45))
* restore download artifact step, support multi-line tags ([#90](https://github.com/ublue-os/base/issues/90)) ([c40bddf](https://github.com/ublue-os/base/commit/c40bddfdf39a61545700ecb8123a02abd24a4f8f))
* update cosign action ([#94](https://github.com/ublue-os/base/issues/94)) ([0aff9ba](https://github.com/ublue-os/base/commit/0aff9bac374c3494f57a360fd4426afe705bfee9))

## 1.0.0 (2023-02-04)


### Features

* Add code-of-conduct ([#39](https://github.com/ublue-os/base/issues/39)) ([aab8078](https://github.com/ublue-os/base/commit/aab8078cfdc7d2354e057a0ca4771d3a53d2df4c))
* add conventional commit linting and release notes generator ([b7820b4](https://github.com/ublue-os/base/commit/b7820b4ba312ca939d0dc977ed9f6a08d135324b))
* tag PR builds independently from matrix.version, latest, and stable ([b022183](https://github.com/ublue-os/base/commit/b02218386235e6d40a11a48b5b1171e9acf8d1eb))


### Bug Fixes

* Don't generate an image when README.md is updated ([#36](https://github.com/ublue-os/base/issues/36)) ([8c170cf](https://github.com/ublue-os/base/commit/8c170cfe89dd306eec0940f4dc50ed245c94bc2b))
* only generate date tag for main branch ([94aa5bb](https://github.com/ublue-os/base/commit/94aa5bb8df2aac0985d4c9422b19b0c03a3f25b0))
