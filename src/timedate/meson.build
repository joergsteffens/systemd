if conf.get('ENABLE_TIMEDATED') == 1
        install_data('org.freedesktop.timedate1.conf',
                     install_dir : dbuspolicydir)
        install_data('org.freedesktop.timedate1.service',
                     install_dir : dbussystemservicedir)

        i18n.merge_file(
                'org.freedesktop.timedate1.policy',
                input : 'org.freedesktop.timedate1.policy.in',
                output : 'org.freedesktop.timedate1.policy',
                po_dir : po_dir,
                data_dirs : po_dir,
                install : install_polkit,
                install_dir : polkitpolicydir)
endif
