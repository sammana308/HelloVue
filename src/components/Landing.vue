<template>
	<v-container fill-height>
		<v-responsive max-width="425" class="mx-auto">
			<v-row class="text-center">
				<v-col cols="12">
					<v-img
						:src="require('../assets/logo.svg')"
						class="my-3"
						contain
						height="150"
					/>
				</v-col>

				<v-col cols="12" class="mb-4">
					<h1 class="display-1 font-weight-bold mb-3">
						Welcome to Hello World
					</h1>

					<p class="subheading font-weight-regular">
						{{ input }}
					</p>
				</v-col>

				<v-col cols="12">
					<v-text-field
						v-model="input"
						label="Start typing..."
						filled
						rounded
						clearable
					></v-text-field>
				</v-col>
			</v-row>
		</v-responsive>
	</v-container>
</template>

<script>
export default {
	name: "Landing",

	data: () => ({
		input: "",
	}),
};
</script>
