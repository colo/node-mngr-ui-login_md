<template>
  <div id="app">
		<md-layout md-gutter>
			<md-layout><br></md-layout>
		</md-layout>
		<md-layout md-gutter>
			<md-layout md-flex="33"><br></md-layout>
			<md-layout>
				<form novalidate @submit="onSubmit">

				<md-card md-with-hover>
					<md-card-header>
						<div class="md-title">Login:</div>
					</md-card-header>

					<md-card-content>
						<md-input-container>
							<md-icon class="md-primary">
								account_box
								<md-tooltip>Registered user</md-tooltip>
							</md-icon>
							<label>User</label>
							<md-input id="username" v-model="username"></md-input>
						</md-input-container>
						
						<md-input-container md-has-password>
							<md-icon class="md-primary">
								vpn_key
								<md-tooltip>Password</md-tooltip>
							</md-icon>
							<label>Password</label>
							<md-input id="password" v-model="password" type="password"></md-input>
						</md-input-container>
						
						
					</md-card-content>

					<md-card-actions>
						<md-button type="submit" class="md-raised md-primary">Login</md-button>
					</md-card-actions>
				</md-card>
				</form>
				
			</md-layout>
			<md-layout md-flex="33"><br></md-layout>
		</md-layout>

		
  </div>
</template>

<script src='./models/login.js'></script>

<style src="vue-material/dist/vue-material.css"></style>
