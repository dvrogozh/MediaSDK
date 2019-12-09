This directory contains a copy of the Linux kernel include/drm/i915_pciids.h
file required by mediasdk to recognize and identify underlying Intel platform.
Whenever mediasdk needs new PCI ID definitions, this file should be updated.

These files in master should only be updated once the changes have landed
in the drm-next tree (see https://cgit.freedesktop.org/drm/drm/).

You can copy file directly from the kernel:

    cp ${KERNEL_TREE}/include/drm/i915_pciids.h ${MSDK_TREE}/contrib/drm/

The last update was done at the following kernel commit :

    commit e42617b825f8073569da76dc4510bfa019b1c35a
    Author: Linus Torvalds <torvalds@linux-foundation.org>
    Date:   Sun Dec 8 14:57:55 2019 -0800

        Linux 5.5-rc1
