<script>
    let notice = [
        {
            date : "2024-Mar-15, Fri",
            desc : "Revised Routine of Back Exam (BE/BAR All Year I Part) for 2081 Baishakh",
        },
        {
            date : "2024-Mar-15, Fri",
            desc : "Revised Routine of Back Exam (BE/BAR All Year I Part) for 2081 Baishakh",
        },
        {
            date : "2024-Mar-15, Fri",
            desc : "Revised Routine of Back Exam (BE/BAR All Year I Part) for 2081 Baishakh",
        },
        {
            date : "2024-Mar-15, Fri",
            desc : "Revised Routine of Back Exam (BE/BAR All Year I Part) for 2081 Baishakh",
        },
        {
            date : "2024-Mar-15, Fri",
            desc : "Revised Routine of Back Exam (BE/BAR All Year I Part) for 2081 Baishakh",
        },
        {
            date : "2024-Mar-15, Fri",
            desc : "Revised Routine of Back Exam (BE/BAR All Year I Part) for 2081 Baishakh",
        },
        {
            date : "2024-Mar-15, Fri",
            desc : "Revised Routine of Back Exam (BE/BAR All Year I Part) for 2081 Baishakh",
        },
    ];
</script>
<main class="px-10 font-inter my-20">
    <div class="text-2xl text-[#10152E] font-medium text-center my-5">Notices</div>
    <div>
        <table class="mx-auto my-4">
            <thead>
                <tr class="border bg-gray-300">
                    <th class="py-2">Date</th>
                    <th class="py-2">Title</th>
                    <th class="py-2">Action</th>
                </tr>
            </thead>
            <tbody>
                {#each notice as item}
                    <tr class="border ">
                        <td class="px-4 py-3 w-fit">{item.date}</td>
                        <td class="px-4 py-3 font-medium"><a href>{item.desc}</a></td>
                        <td class="px-4 py-3"><a href>View Details</a></td>
                    </tr>
                {/each}
            </tbody>
        </table>
    </div>
</main>