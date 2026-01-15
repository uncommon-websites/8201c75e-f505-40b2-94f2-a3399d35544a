<script>
	let openIndex = 0;
	const faqs = [
		{
			question: "Who is HiPeople for?",
			answer: "HiPeople is designed for mid-market and enterprise talent teams who need to scale their hiring without compromising on quality. It's especially powerful for teams drowning in manual screening and reference check work."
		},
		{
			question: "How does the AI screening work?",
			answer: "Our AI analyzes candidate profiles and resumes against your specific job requirements, scoring them based on skills, experience, and potential. It surfaces the best matches so you can focus your time on high-potential candidates."
		},
		{
			question: "Is HiPeople compliant and secure?",
			answer: "Yes. We are SOC 2 Type II certified and GDPR compliant. Security and data privacy are at the core of our platform, making us a trusted partner for enterprise HR teams."
		},
		{
			question: "How long do reference checks take?",
			answer: "While manual reference checks can take days or weeks, HiPeople automates the process, often delivering structured feedback in just a few hours."
		},
		{
			question: "Does it integrate with my ATS?",
			answer: "Absolutely. We offer deep integrations with Greenhouse, Lever, Workday, SmartRecruiters, Ashby, and many more, ensuring HiPeople fits seamlessly into your existing workflow."
		},
		{
			question: "Can I customize the assessments?",
			answer: "Yes, you can choose from our library of validated assessments or work with us to create custom evaluations tailored to your specific role requirements."
		}
	];
</script>

<section class="py-24">
	<div class="mx-auto max-w-[1400px] px-6">
		<div class="grid grid-cols-1 gap-16 lg:grid-cols-12">
			<!-- Left Side -->
			<div class="lg:col-span-4">
				<div class="mb-4 text-[10px] font-bold tracking-widest text-gray-400 uppercase">[06] FAQ</div>
				<h2 class="mb-6 text-4xl font-bold tracking-tight text-gray-900">Your questions, answered</h2>
				<p class="mb-8 text-lg leading-relaxed text-gray-600">
					We're here to help. Reach out to our team for guidance on how to integrate HiPeople into your hiring workflow.
				</p>
				<a href="#" class="inline-block bg-gray-900 px-8 py-4 text-[11px] font-bold tracking-widest text-white transition-all hover:bg-primary-600 uppercase">
					Book a Demo
				</a>
			</div>

			<!-- Right Side (Accordion) -->
			<div class="lg:col-span-8">
				<div class="divide-y divide-gray-200 border-t border-b border-gray-200">
					{#each faqs as faq, i}
						<div class="group">
							<button 
								class="flex w-full items-center justify-between py-6 text-left focus:outline-none"
								onclick={() => openIndex = openIndex === i ? -1 : i}
							>
								<span class="text-lg font-medium text-gray-900">{faq.question}</span>
								<span class="ml-4 flex h-6 w-6 items-center justify-center text-gray-400">
									{#if openIndex === i}
										<svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M18 6L6 18M6 6l12 12"/></svg>
									{:else}
										<svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 5v14M5 12h14"/></svg>
									{/if}
								</span>
							</button>
							{#if openIndex === i}
								<div class="pb-6 text-gray-600 leading-relaxed">
									{faq.answer}
								</div>
							{/if}
						</div>
					{/each}
				</div>
			</div>
		</div>
	</div>
</section>