<script lang="ts">
    import AppContent from '@/components/app-content.svelte';
    import AppHeader from '@/components/app-header.svelte';
    import AppShell from '@/components/app-shell.svelte';
    import type { BreadcrumbItemType } from '@/types';
    import type { Snippet } from 'svelte';

    interface Props {
        breadcrumbs?: BreadcrumbItemType[];
        children?: Snippet;
    }

    let { breadcrumbs = [], children }: Props = $props();
</script>

<AppShell variant="header">
    <AppHeader {breadcrumbs} />
    <AppContent variant="header">
        {@render children?.()}
    </AppContent>
</AppShell>
