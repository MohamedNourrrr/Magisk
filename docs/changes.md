
# Magisk Changelog

### v26.1

- [App] Fix crashing when revoking root permissions
- [MagiskInit] Always prefer `ext4` partitions over `f2fs` when selecting the pre-init partition
- [General] Restore module files' context/owner/group from mirror. This is a regression introduced in v26.0

### v26.0

- [General] Bump minimum supported Android version to Android 6.0
- [General] New magic mount backend. It supports loading modules into system with `overlayfs` files injected
- [Zygisk] Release new API version 4
- [Zygisk] Prevent crashing daemon in error
- [Zygisk] Rewrite zygote code injection with new loader library approach
- [Zygisk] Rewrite code unloading implementation
- [MagiskBoot] Support amonet microloader devices
- [MagiskBoot] Always use lz4_legacy compression on v4 boot images. This fixes boot image patching issues on Android U preview.
