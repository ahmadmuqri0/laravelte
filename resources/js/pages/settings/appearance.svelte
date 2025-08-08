<script lang="ts">
    import AppearanceTabs from '@/components/appearance-tabs.svelte';
    import HeadingSmall from '@/components/heading-small.svelte';
    import { type BreadcrumbItem } from '@/types';

    import AppLayout from '@/layouts/app-layout.svelte';
    import SettingsLayout from '@/layouts/settings/layout.svelte';

    const breadcrumbItems: BreadcrumbItem[] = [
        {
            title: 'Appearance settings',
            href: '/settings/appearance',
        },
    ];
</script>

<svelte:head>
    <title>Appearance Settings</title>
</svelte:head>

<AppLayout breadcrumbs={breadcrumbItems}>
    <SettingsLayout>
        <div class="space-y-6">
            <HeadingSmall title="Appearance settings" description="Update your account's appearance settings" />
            <AppearanceTabs />
        </div>
    </SettingsLayout>
</AppLayout>
