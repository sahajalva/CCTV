<script>
	let com = [
		{ name: 'home', svg: '<svg xmlns="http://www.w3.org/2000/svg" data-name="Layer 1" viewBox="0 0 32 32"><path d="M25,31H7a3,3,0,0,1-3-3V16H2a1,1,0,0,1-.68-1.73L14,2.53h0a3,3,0,0,1,4.08,0L30.68,14.27A1,1,0,0,1,30,16H28V28A3,3,0,0,1,25,31ZM4.55,14H5a1,1,0,0,1,1,1V28a1,1,0,0,0,1,1H25a1,1,0,0,0,1-1V15a1,1,0,0,1,1-1h.45L16.68,4a1,1,0,0,0-1.36,0Z"/></svg>'},
		{ name: 'stakeholder', svg: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 64 64"><path d="M57,27c-.06409,0-.1236.01654-.18707.01892l-3.84143-8.963c5.07158-4.74567-2.06952-12.06483-6.94825-7.12378L36.96863,7.3103a4.98236,4.98236,0,1,0-9.94971-.12323l-8.963,3.84143c-2.88977-3.48885-8.82233-1.21734-8.73357,3.29388a5.02494,5.02494,0,0,0,7.80516,4.13551,16.29747,16.29747,0,0,0,1.47736,1.561c-7.25049,7.81261-5.62036,20.8515,3.12016,26.73922,11.68676,8.28058,28.28628-.22652,28.27492-14.75829.054-15.48661-18.63659-23.737-29.981-13.395a16.252,16.252,0,0,0-1.561-1.47736,4.906,4.906,0,0,0,.59747-4.35211L27.507,9.15308a4.98659,4.98659,0,0,0,8.93182.09961L44.97711,12.668a4.99141,4.99141,0,0,0,6.2475,6.38739L54.84692,27.507a4.98659,4.98659,0,0,0-.09961,8.93182L51.332,44.97711a4.99141,4.99141,0,0,0-6.38739,6.2475L36.493,54.84692a4.98659,4.98659,0,0,0-8.93182-.09961L19.02289,51.332a4.99141,4.99141,0,0,0-6.2475-6.38739L9.15308,36.493A4.99933,4.99933,0,0,0,6.99987,27c-6.74765.256-6.5469,10.02419.1872,9.98106l3.84143,8.963c-5.07158,4.74567,2.06952,12.06483,6.94825,7.12378l9.05462,3.62183a4.98236,4.98236,0,1,0,9.94971.12323l8.963-3.84143c4.74567,5.07158,12.06483-2.06952,7.12378-6.94825l3.62183-9.05462C63.49985,37.19146,63.82615,27.26261,57,27ZM12.20117,16.44336a2.99986,2.99986,0,0,1,4.24225-4.24212A2.99986,2.99986,0,0,1,12.20117,16.44336ZM23.43073,45.48877A8.09091,8.09091,0,0,1,29.2204,40.116a3.00035,3.00035,0,0,0,5.55176-.00153,8.09061,8.09061,0,0,1,5.79711,5.37433A16.03859,16.03859,0,0,1,23.43073,45.48877ZM32,36a8.00917,8.00917,0,0,1-8-8c.43956-10.61307,15.56206-10.61,16,.00006A8.00919,8.00919,0,0,1,32,36Zm0,2c.33752,0,.671-.01788,1-.05072V39a1.00067,1.00067,0,0,1-1,1,1.01519,1.01519,0,0,1-1-1.05957v-.99115C31.329,37.98212,31.66248,38,32,38Zm16-6a15.96718,15.96718,0,0,1-5.7276,12.25006A10.1301,10.1301,0,0,0,35,38.09943V37.5387C45.75429,33.96149,43.4684,18.23561,31.99985,18,20.52957,18.23663,18.2474,33.96352,29,37.5387v.56073a10.1301,10.1301,0,0,0-7.2724,6.15063,16.04145,16.04145,0,0,1-.97117-23.61713C30.647,10.70584,48.03546,17.83417,48,32ZM32,10a3.00019,3.00019,0,0,1,.00009-6A3.00019,3.00019,0,0,1,32,10Zm15.55664,6.44336a2.99986,2.99986,0,0,1,4.24225-4.24212A2.99986,2.99986,0,0,1,47.55664,16.44336ZM4,32a3.00019,3.00019,0,0,1,6,.00009A3.00019,3.00019,0,0,1,4,32Zm8.20117,19.79883a2.99986,2.99986,0,0,1,4.24225-4.24212A2.99986,2.99986,0,0,1,12.20117,51.79883ZM32,60a3.00019,3.00019,0,0,1,.00009-6A3.00019,3.00019,0,0,1,32,60Zm19.79883-8.20117a2.99994,2.99994,0,0,1-4.24212-4.24226A2.99994,2.99994,0,0,1,51.79883,51.79883ZM57,35a3.00019,3.00019,0,0,1,.00009-6A3.00019,3.00019,0,0,1,57,35Z"/></svg>'},
		{ name: 'webinar', svg: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 64 64"><path d="M59,44H58V11a3,3,0,0,0-3-3H9a3,3,0,0,0-3,3V44H5a3,3,0,0,0-3,3v2a7,7,0,0,0,7,7H55a7,7,0,0,0,7-7V47A3,3,0,0,0,59,44ZM8,11a1,1,0,0,1,1-1H55a1,1,0,0,1,1,1V44H8ZM35.41,47.24a1,1,0,0,1-1,.76H29.56a1,1,0,0,1-1-.76L28.28,46h7.44Z"/><path d="M22.22 26.79a5 5 0 1 0-6.44 0A7 7 0 0 0 12 33v4a3 3 0 0 0 3 3h8a3 3 0 0 0 3-3V33A7 7 0 0 0 22.22 26.79zM16 23a3 3 0 1 1 3 3A3 3 0 0 1 16 23zm8 14a1 1 0 0 1-1 1H15a1 1 0 0 1-1-1V33a5 5 0 0 1 10 0zM49 14H33a3 3 0 0 0-3 3V33a3 3 0 0 0 3 3H49a3 3 0 0 0 3-3V17A3 3 0 0 0 49 14zM36 19h4a1 1 0 0 1 0 2H36a1 1 0 0 1 0-2zM46 31H36a1 1 0 0 1 0-2H46a1 1 0 0 1 0 2zm0-5H36a1 1 0 0 1 0-2H46a1 1 0 0 1 0 2z"/></svg>'},
		{ name: 'research', svg: '<svg xmlns="http://www.w3.org/2000/svg" data-name="Layer 1" viewBox="0 0 24 24"><path d="M21.07,16.83,19,14.71a3.08,3.08,0,0,0-3.4-.57l-.9-.9a7,7,0,1,0-1.41,1.41l.89.89A3,3,0,0,0,14.71,19l2.12,2.12a3,3,0,0,0,4.24,0A3,3,0,0,0,21.07,16.83Zm-8.48-4.24a5,5,0,1,1,0-7.08A5,5,0,0,1,12.59,12.59Zm7.07,7.07a1,1,0,0,1-1.42,0l-2.12-2.12a1,1,0,0,1,0-1.42,1,1,0,0,1,1.42,0l2.12,2.12A1,1,0,0,1,19.66,19.66Z"/></svg>'},
		{ name: "gallery", svg: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><g data-name="katman 2"><polyline fill="none" stroke="#2c2c2c" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" points="22.41 19.41 17 14 14.5 16.5"/><polyline fill="none" stroke="#2c2c2c" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" points="18 20 9.5 11.5 1.59 19.41"/><rect width="22" height="16" x="1" y="4" fill="none" stroke="#2c2c2c" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" rx="2" ry="2"/><circle cx="17" cy="9" r="1" fill="none" stroke="#2c2c2c" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"/><rect width="24" height="24" fill="none"/></g></svg>'},
		{ name: 'team', svg: '<svg class="svg-icon" style="width: 1em; height: 1em;vertical-align: middle;fill: currentColor;overflow: hidden;" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg"><path d="M629.956 486.519c44.718-34.903 73.61-88.978 73.61-149.734 0-105.01-85.99-190.453-191.72-190.453s-191.72 85.444-191.72 190.453c0 60.756 28.886 114.83 73.609 149.734-117.862 46.786-201.415 161.14-201.415 294.66v63.467c0 17.554 14.295 31.75 31.943 31.75h575.16c17.653 0 31.944-14.196 31.944-31.75V781.18c0.001-133.572-83.552-247.876-201.411-294.661zM373.152 336.534c0-75.995 62.198-137.774 138.694-137.774 76.492 0 138.693 61.78 138.693 137.774 0 75.976-62.2 137.774-138.693 137.774-76.496 0-138.694-61.773-138.694-137.774z m410.165 487.78h-542.97v-33.713c0-148.708 121.79-269.705 271.523-269.705 149.68 0 271.447 120.997 271.447 269.705v33.713zM264.212 515.95l6.24-1.489c13.4-4.453 22.945-16.136 22.945-29.858 0-13.253-8.924-24.586-21.575-29.36-34.212-15.44-56.284-49.323-56.284-86.663 0-42.311 36.768-77.958 75.251-90.315 6.737-20.659 16.928-39.777 29.904-56.681a214.079 214.079 0 0 1 7.137-10.963c-2.584-0.124-5.045-0.768-7.703-0.768-88.083 0-159.775 71.196-159.775 158.728 0 40.175 15.41 77.838 41.564 106.478C118.734 517.866 64.49 603.482 64.49 700.339v49.096c0 17.553 14.296 31.745 31.944 31.745h57.25c0-21.75 2.24-35.695 6.44-56.208h-40.446V700.34c0-87.736 59.365-163.034 144.535-184.39z m557.213-40.892c26.155-28.64 41.565-66.303 41.565-106.478 0-87.533-71.67-158.756-159.776-158.756-2.66 0-5.12 0.649-7.704 0.771a213.392 213.392 0 0 1 7.137 10.963c12.978 16.904 23.167 36.022 29.881 56.683 38.484 12.352 80.57 48.004 80.57 90.314 0 37.341-22.101 71.248-56.284 86.664-12.655 4.77-21.58 16.107-21.58 29.36 0 13.723 9.574 25.406 22.946 29.853l6.24 1.493c85.199 21.38 144.536 96.655 144.536 184.413v24.632h-45.79c4.225 20.514 6.44 34.458 6.44 56.209h57.25c17.677 0 31.945-14.192 31.945-31.745v-49.096c0.052-96.856-54.193-182.472-137.376-225.28z m0 0"  /></svg>'},
		{ name: "knowledge", svg: '<svg xmlns="http://www.w3.org/2000/svg" data-name="Layer 1" viewBox="0 0 64 64"><path d="M3 62H19a1 1 0 0 0 1-1V57a9.01 9.01 0 0 0-5.623-8.337 5 5 0 1 0-6.754 0A9.01 9.01 0 0 0 2 57v4A1 1 0 0 0 3 62zm8-20a3 3 0 1 1-3 3A3 3 0 0 1 11 42zM4 57a7 7 0 0 1 14 0v3H4zM58.814 3.091H55.729a7.011 7.011 0 0 0-7.458 0h-.542a7.011 7.011 0 0 0-7.458 0H37.186A3.293 3.293 0 0 0 34 6.476V15a1 1 0 0 0 1 1H61a1 1 0 0 0 1-1V6.476A3.293 3.293 0 0 0 58.814 3.091zM36 14V6.476a1.3 1.3 0 0 1 1.186-1.385H39v8.818c0 .031.011.06.013.091zm5.576 0a4.963 4.963 0 0 1 4.848 0zM47 12.035a7.061 7.061 0 0 0-6 0V5.01a4.951 4.951 0 0 1 6 0zM49.576 14a4.963 4.963 0 0 1 4.848 0zM55 12.035a7.061 7.061 0 0 0-6 0V5.01a4.951 4.951 0 0 1 6 0zM60 14H56.987c0-.031.013-.06.013-.091V5.091h1.814A1.3 1.3 0 0 1 60 6.476z"/><path d="M52.5,27h-40a8.5,8.5,0,0,1,0-17H32V8H12.5a10.5,10.5,0,0,0,0,21h40a7.5,7.5,0,0,1,0,15H18v2H52.5a9.5,9.5,0,0,0,0-19Z"/></svg>'},
		{ name: 'media', svg: '<svg xmlns="http://www.w3.org/2000/svg" width="26" height="26" viewBox="0 0 26 26"><path d="M 13 0 C 5.8262428 0 3e-005 5.8262 0 13 C -2.7e-005 20.1738 5.8262018 26 13 26 C 20.173798 26 26.000028 20.1738 26 13 C 25.99997 5.8262 20.173758 0 13 0 z M 13 1 C 19.633268 1 24.999973 6.3667 25 13 C 25.000026 19.6333 19.633306 25 13 25 C 6.3666948 25 0.999975 19.6333 1 13 C 1.0000279 6.3667 6.3667328 1 13 1 z M 6 6 L 6 6.5 L 6 16 L 12.5 16 L 12.5 18.546875 L 10.699219 19.898438 L 10.300781 20.197266 L 10.900391 20.998047 L 11.300781 20.697266 L 12.5 19.796875 L 12.5 20.5 L 12.5 21 L 13.5 21 L 13.5 20.5 L 13.5 19.796875 L 14.699219 20.697266 L 15.099609 20.998047 L 15.699219 20.197266 L 15.300781 19.898438 L 13.5 18.546875 L 13.5 16 L 20 16 L 20 6 L 6 6 z M 7 7 L 19 7 L 19 15 L 7 15 L 7 7 z M 12.015625 8.6113281 L 12.015625 9.5 L 12.015625 13.388672 L 15.949219 11 L 12.015625 8.6113281 z M 13.015625 10.388672 L 14.023438 11.001953 L 13.015625 11.613281 L 13.015625 10.388672 z " color="#000" font-family="sans-serif" font-weight="400" overflow="visible" style="line-height:normal;text-indent:0;text-align:start;text-decoration-line:none;text-decoration-style:solid;text-decoration-color:#000;text-transform:none;block-progression:tb;isolation:auto;mix-blend-mode:normal"/></svg>'}
		];
</script>
<aside class="w-16 flex-col">
	<div class="fixed top-0 left-0 h-screen w-16 flex flex-col bg-white dark:bg-gray-900 shadow-lg">
		<div
			class=" @apply relative flex items-center justify-center h-12 w-12 mt-2 mb-2 mx-auto    bg-gray-400 hover:scale-125 dark:bg-gray-800 text-orange-500 hover:text-white
        hover:rounded-xl rounded-3xl transition-all duration-300 ease-linear  cursor-pointer shadow-lg  group"
		>
			<svg xmlns="http://www.w3.org/2000/svg" width="36" height="36" viewBox="0 0 36 36"
				><g transform="translate(0 -1016.362)"
					><rect width="36" height="36" y="1016.362" fill="#f05542" rx="6" ry="6" /><g
						transform="translate(253.5 -340)"
						><rect
							width="28"
							height="21"
							x="-248"
							y="1362.362"
							color="#000"
							opacity=".15"
							overflow="visible"
							rx="1.4"
							ry="1.4"
							style="isolation:auto;mix-blend-mode:normal"
						/><rect
							style="isolation:auto;mix-blend-mode:normal"
							width="28"
							height="21"
							x="-253"
							y="1366.362"
							color="#000"
							opacity=".15"
							overflow="visible"
							rx="1.4"
							ry="1.4"
						/><rect
							style="isolation:auto;mix-blend-mode:normal"
							width="28"
							height="21"
							x="-247"
							y="1362.362"
							fill="#f8b84e"
							color="#000"
							overflow="visible"
							rx="1.4"
							ry="1.4"
						/><path
							d="m -239.6,1367.9155 c 0,1.5464 -1.25331,2.8029 -2.8,2.8029 -1.54669,0 -2.8,-1.2565 -2.8,-2.8029 0,-1.5468 1.25331,-2.7971 2.8,-2.7971 1.54669,0 2.8,1.2503 2.8,2.7971 z"
							opacity=".15"
						/><path
							fill="#e9eded"
							d="m -238.6,1367.9155 c 0,1.5464 -1.2533,2.8029 -2.8,2.8029 -1.54669,0 -2.8,-1.2565 -2.8,-2.8029 0,-1.5468 1.25331,-2.7971 2.8,-2.7971 1.5467,0 2.8,1.2503 2.8,2.7971 z"
						/><path
							fill="#2b4255"
							d="m -231.43095,1368.1907 c 0.34724,0.039 0.70947,0.1999 0.98984,0.4815 l 0.014,0.014 3.30585,3.6829 1.59688,-1.7801 0.014,-0.014 c 0.24839,-0.2483 0.59805,-0.4519 1.02539,-0.4757 0.42734,-0.024 0.88866,0.1645 1.23868,0.5141 l 0.0218,0.022 1.42187,1.6871 0,6.5789 c 9.8e-4,0.017 0.003,0.035 0.003,0.049 l 0,0.071 -0.003,0.017 0,1.5231 -0.7,0 c -0.36508,0 -0.56287,0 -0.90508,0 l -0.0602,0 -9.43086,0 -6.8332,0 -0.0574,0 c -0.88117,0 -1.61066,-0.7269 -1.61066,-1.6079 0,-0.3406 0.0904,-0.6285 0.20234,-0.8257 0.0349,-0.06 0.0675,-0.099 0.10122,-0.1423 l 0.0112,-0.028 0.0519,-0.057 c 0.0188,-0.021 0.0318,-0.029 0.041,-0.043 0.0126,-0.014 0.0112,-0.014 0.008,-0.014 l 8.18125,-9.1273 0.014,-0.014 c 0.33476,-0.3347 0.71192,-0.5086 1.01993,-0.5086 0.10864,-0.014 0.22332,-0.015 0.33905,0 z"
							color="#000"
							overflow="visible"
							style="isolation:auto;mix-blend-mode:normal"
						/><rect
							width="28"
							height="21"
							x="-252"
							y="1366.362"
							fill="#25b39e"
							color="#000"
							overflow="visible"
							rx="1.4"
							ry="1.4"
							style="isolation:auto;mix-blend-mode:normal"
						/><path
							d="m -244.6,1371.9155 c 0,1.5464 -1.25331,2.8029 -2.8,2.8029 -1.54669,0 -2.8,-1.2565 -2.8,-2.8029 0,-1.5468 1.25331,-2.7971 2.8,-2.7971 1.54669,0 2.8,1.2503 2.8,2.7971 z"
							opacity=".15"
						/><path
							d="m -237.43095,1372.1907 c 0.34724,0.039 0.70946,0.1999 0.98984,0.4815 l 0.014,0.014 3.30585,3.6829 1.59688,-1.7801 0.014,-0.014 c 0.24839,-0.2483 0.59805,-0.4519 1.02539,-0.4757 0.42733,-0.024 0.88866,0.1645 1.23868,0.5141 l 0.0218,0.022 1.42186,1.6871 0,6.5789 c 9.8e-4,0.017 0.003,0.035 0.003,0.049 l 0,0.071 -0.003,0.017 0,1.5231 -0.7,0 c -0.36507,0 -0.56287,0 -0.90507,0 l -0.0602,0 -9.43086,0 -6.8332,0 -0.0574,0 c -0.88118,0 -1.61066,-0.7269 -1.61066,-1.6079 0,-0.3406 0.0904,-0.6285 0.20234,-0.8257 0.0349,-0.06 0.0675,-0.099 0.10122,-0.1423 l 0.0112,-0.028 0.0519,-0.057 c 0.0188,-0.021 0.0318,-0.029 0.041,-0.043 0.0126,-0.014 0.0112,-0.014 0.008,-0.014 l 8.18125,-9.1273 0.014,-0.014 c 0.33475,-0.3347 0.71191,-0.5086 1.01993,-0.5086 0.10864,-0.014 0.22331,-0.015 0.33905,0 z"
							color="#000"
							opacity=".15"
							overflow="visible"
							style="isolation:auto;mix-blend-mode:normal"
						/><path
							fill="#e9eded"
							d="m -243.6,1371.9155 c 0,1.5464 -1.25331,2.8029 -2.8,2.8029 -1.54669,0 -2.8,-1.2565 -2.8,-2.8029 0,-1.5468 1.25331,-2.7971 2.8,-2.7971 1.54669,0 2.8,1.2503 2.8,2.7971 z"
						/><path
							fill="#2b4255"
							style="isolation:auto;mix-blend-mode:normal"
							d="m -236.43095,1372.1907 c 0.34724,0.039 0.70946,0.1999 0.98984,0.4815 l 0.014,0.014 3.30585,3.6829 1.59688,-1.7801 0.014,-0.014 c 0.24839,-0.2483 0.59805,-0.4519 1.02539,-0.4757 0.42733,-0.024 0.88866,0.1645 1.23868,0.5141 l 0.0218,0.022 1.42186,1.6871 0,6.5789 c 9.8e-4,0.017 0.003,0.035 0.003,0.049 l 0,0.071 -0.003,0.017 0,1.5231 -0.7,0 c -0.36507,0 -0.56287,0 -0.90507,0 l -0.0602,0 -9.43086,0 -6.8332,0 -0.0574,0 c -0.88118,0 -1.61066,-0.7269 -1.61066,-1.6079 0,-0.3406 0.0904,-0.6285 0.20234,-0.8257 0.0349,-0.06 0.0675,-0.099 0.10122,-0.1423 l 0.0112,-0.028 0.0519,-0.057 c 0.0188,-0.021 0.0318,-0.029 0.041,-0.043 0.0126,-0.014 0.0112,-0.014 0.008,-0.014 l 8.18125,-9.1273 0.014,-0.014 c 0.33476,-0.3347 0.71192,-0.5086 1.01993,-0.5086 0.10864,-0.014 0.22331,-0.015 0.33905,0 z"
							color="#000"
							overflow="visible"
						/></g
					></g
				></svg
			>
			<span
				class="@apply absolute w-auto p-2 m-2 min-w-max left-14 rounded-md shadow-md         text-white bg-gray-900  text-xs font-bold transition-all duration-100 scale-0 origin-left; group-hover:scale-100"
			>
				text
			</span>
		</div>
		<hr
			class="@apply bg-gray-200 w-3/4 mx-auto dark:bg-gray-800 border border-gray-200 dark:border-gray-800 rounded-full mx-2;"
		/>
		<div
			class=" @apply relative flex items-center justify-center h-12 w-12 mt-2 mb-2 mx-auto    bg-gray-400 hover:bg-orange-600 dark:bg-gray-800 text-orange-500 hover:text-white
hover:rounded-xl rounded-3xl    transition-all duration-300 ease-linear  cursor-pointer shadow-lg  group"
		>
			icon
			<span
				class="@apply absolute w-auto p-2 m-2 min-w-max left-14 rounded-md shadow-md         text-white bg-gray-900  text-xs font-bold transition-all duration-100 scale-0 origin-left; group-hover:scale-100"
			>
				text
			</span>
		</div>
		<div
			class=" @apply relative flex items-center justify-center h-12 w-12 mt-2 mb-2 mx-auto    bg-gray-400 hover:bg-orange-600 dark:bg-gray-800 text-orange-500 hover:text-white
hover:rounded-xl rounded-3xl    transition-all duration-300 ease-linear  cursor-pointer shadow-lg  group"
		>
			icon
			<span
				class="@apply absolute w-auto p-2 m-2 min-w-max left-14 rounded-md shadow-md         text-white bg-gray-900  text-xs font-bold transition-all duration-100 scale-0 origin-left; group-hover:scale-100"
			>
				text
			</span>
		</div>
		<div
			class=" @apply relative flex items-center justify-center h-12 w-12 mt-2 mb-2 mx-auto    bg-gray-400 hover:bg-orange-600 dark:bg-gray-800 text-orange-500 hover:text-white
hover:rounded-xl rounded-3xl    transition-all duration-300 ease-linear  cursor-pointer shadow-lg  group"
		>
			icon
			<span
				class="@apply absolute w-auto p-2 m-2 min-w-max left-14 rounded-md shadow-md         text-white bg-gray-900  text-xs font-bold transition-all duration-100 scale-0 origin-left; group-hover:scale-100"
			>
				text
			</span>
		</div>
		<div
			class=" @apply relative flex items-center justify-center h-12 w-12 mt-2 mb-2 mx-auto    bg-gray-400 hover:bg-orange-600 dark:bg-gray-800 text-orange-500 hover:text-white
hover:rounded-xl rounded-3xl    transition-all duration-300 ease-linear  cursor-pointer shadow-lg  group"
		>
			icon
			<span
				class="@apply absolute w-auto p-2 m-2 min-w-max left-14 rounded-md shadow-md         text-white bg-gray-900  text-xs font-bold transition-all duration-100 scale-0 origin-left; group-hover:scale-100"
			>
				text
			</span>
		</div>
		<div
			class=" @apply relative flex items-center justify-center h-12 w-12 mt-2 mb-2 mx-auto    bg-gray-400 hover:bg-orange-600 dark:bg-gray-800 text-orange-500 hover:text-white
hover:rounded-xl rounded-3xl    transition-all duration-300 ease-linear  cursor-pointer shadow-lg  group"
		>
			icon
			<span
				class="@apply absolute w-auto p-2 m-2 min-w-max left-14 rounded-md shadow-md         text-white bg-gray-900  text-xs font-bold transition-all duration-100 scale-0 origin-left; group-hover:scale-100"
			>
				text
			</span>
		</div>
		<div
			class=" @apply relative flex items-center justify-center h-12 w-12 mt-2 mb-2 mx-auto    bg-gray-400 hover:bg-orange-600 dark:bg-gray-800 text-orange-500 hover:text-white
hover:rounded-xl rounded-3xl    transition-all duration-300 ease-linear  cursor-pointer shadow-lg  group"
		>
			icon
			<span
				class="@apply absolute w-auto p-2 m-2 min-w-max left-14 rounded-md shadow-md         text-white bg-gray-900  text-xs font-bold transition-all duration-100 scale-0 origin-left; group-hover:scale-100"
			>
				text
			</span>
		</div>
		<div
			class=" @apply relative flex items-center justify-center h-12 w-12 mt-2 mb-2 mx-auto    bg-gray-400 hover:bg-orange-600 dark:bg-gray-800 text-orange-500 hover:text-white
hover:rounded-xl rounded-3xl    transition-all duration-300 ease-linear  cursor-pointer shadow-lg  group"
		>
			icon
			<span
				class="@apply absolute w-auto p-2 m-2 min-w-max left-14 rounded-md shadow-md         text-white bg-gray-900  text-xs font-bold transition-all duration-100 scale-0 origin-left; group-hover:scale-100"
			>
				text
			</span>
		</div>
	</div>
</aside>
