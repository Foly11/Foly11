- 👋 Hi, I’m @Foly11
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Foly11/Foly11 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<?xml version="1.0" encoding="utf-8" ?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android" android:compileSdkVersion="30" android:compileSdkVersionCodename="11" android:versionCode="28" android:versionName="stb_2.6.1" package="com.ngc.fasttv" platformBuildVersionCode="30" platformBuildVersionName="11">
	<uses-sdk android:minSdkVersion="19" android:targetSdkVersion="30" />
	<meta-data android:name="io.futurestud.tutorials.glide.glidemodule.UnsafeOkHttpClient" android:value="GlideModule" />
	<uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION" />
	<uses-permission android:name="android.permission.ACCESS_FINE_LOCATION" />
	<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
	<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />
	<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE" />
	<uses-permission android:name="android.permission.INTERNET" />
	<uses-permission android:name="android.permission.ACCESS_WIFI_STATE" />
	<uses-permission android:name="android.permission.READ_PHONE_STATE" />
	<uses-permission android:name="android.permission.INSTALL_PACKAGES" />
	<uses-permission android:name="android.permission.REQUEST_INSTALL_PACKAGES" />
	<uses-permission android:name="android.permission.WAKE_LOCK" />
	<uses-permission android:name="com.google.android.finsky.permission.BIND_GET_INSTALL_REFERRER_SERVICE" />
	<uses-permission android:name="com.google.android.c2dm.permission.RECEIVE" />
	<application android:appComponentFactory="androidx.core.app.CoreComponentFactory" android:hardwareAccelerated="true" android:icon="@mipmap/ic_launcher_my_tv_pls" android:label="@string/app_name" android:largeHeap="true" android:name="com.ngc.fasttv.FastTvApplication" android:requestLegacyExternalStorage="true" android:roundIcon="@mipmap/ic_launcher_my_tv_pls_round" android:theme="@style/AppTheme" android:usesCleartextTraffic="true">
		<activity android:name="com.ngc.fasttv.activity.noConnection.NoInternetConnectivityActivity" />
		<activity android:configChanges="keyboard|keyboardHidden|navigation" android:exported="true" android:name="com.ngc.fasttv.test.TestingActivity" />
		<activity android:name="com.ngc.fasttv.test.helper.TvChannelPlayerHelperActivity" android:screenOrientation="landscape" />
		<meta-data android:name="JW_LICENSE_KEY" android:value="EKMaPtmyPdU0nO0cr38EH6xAFPy2cie7iYMfIU4W9zkiUn6QBsyUAKM6eMVAX2hv" />
		<activity android:configChanges="keyboard|keyboardHidden|orientation|screenSize" android:name="com.ngc.fasttv.test.jwPlayer.TvChannelJWPlayerActivity" />
		<activity android:name="com.ngc.fasttv.activity.TvChannelPlayerExo.TvChannelExoPlayerActivity" />
		<activity android:name="com.ngc.fasttv.activity.splashScreen.SplashScreenActivity" android:screenOrientation="landscape" android:supportsRtl="false">
			<intent-filter>
				<action android:name="android.intent.action.MAIN" />
				<category android:name="android.intent.category.LAUNCHER" />
			</intent-filter>
		</activity>
		<activity android:name="com.ngc.fasttv.activity.moviePlayer.PlayerActivity" android:screenOrientation="landscape" android:supportsRtl="false" />
		<activity android:name="com.ngc.fasttv.activity.serviceVersionActivity.PlayServiceVersionActivity" android:screenOrientation="landscape" android:supportsRtl="false" />
		<activity android:label="@string/title_activity_tv_channel_player" android:name="com.ngc.fasttv.activity.tvChannelPlayer.TvChannelPlayerActivity" android:screenOrientation="landscape" />
		<activity android:name="com.ngc.fasttv.activity.tvSeries.TvSeriesDetailActivity" android:screenOrientation="landscape" android:supportsRtl="false" />
		<activity android:name="com.ngc.fasttv.activity.movie.MovieDetailActivity" android:screenOrientation="landscape" android:supportsRtl="false" />
		<activity android:label="@string/app_name" android:name="com.ngc.fasttv.activity.main.MainActivity" android:screenOrientation="landscape" android:supportsRtl="false" android:windowSoftInputMode="stateHidden" />
		<activity android:label="@string/app_name" android:name="com.ngc.fasttv.activity.noConnection.NoConnectionActivity" android:screenOrientation="landscape" android:supportsRtl="false" />
		<activity android:label="@string/app_name" android:name="com.ngc.fasttv.activity.errorActivity.ErrorActivity" android:screenOrientation="landscape" android:supportsRtl="false" />
		<activity android:label="@string/app_name" android:name="com.ngc.fasttv.activity.tutorial.TutorialPlayServiceActivity" android:screenOrientation="landscape" android:supportsRtl="false" />
		<activity android:label="@string/app_name" android:name="com.ngc.fasttv.activity.tutorial.TutorialMyTvInstallActivity" android:screenOrientation="landscape" android:supportsRtl="false" />
		<service android:exported="false" android:name="com.ngc.fasttv.service.AttackReporterService" />
		<receiver android:name="com.ngc.fasttv.receiver.NetworkBroadcastReceiver">
			<intent-filter>
				<action android:name="android.net.conn.CONNECTIVITY_CHANGE" />
				<action android:name="android.net.wifi.WIFI_STATE_CHANGED" />
			</intent-filter>
		</receiver>
		<provider android:authorities="com.ngc.fasttv.provider" android:exported="false" android:grantUriPermissions="true" android:name="androidx.core.content.FileProvider">
			<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@xml/provider_paths" />
		</provider>
		<meta-data android:name="com.bumptech.glide.integration.okhttp3.OkHttpGlideModule" android:value="GlideModule" />
		<service android:directBootAware="true" android:exported="false" android:name="com.google.firebase.components.ComponentDiscoveryService">
			<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.CrashlyticsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar" />
			<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.RemoteConfigRegistrar" android:value="com.google.firebase.components.ComponentRegistrar" />
			<meta-data android:name="com.google.firebase.components:com.google.firebase.messaging.FirebaseMessagingRegistrar" android:value="com.google.firebase.components.ComponentRegistrar" />
			<meta-data android:name="com.google.firebase.components:com.google.firebase.datatransport.TransportRegistrar" android:value="com.google.firebase.components.ComponentRegistrar" />
			<meta-data android:name="com.google.firebase.components:com.google.firebase.iid.Registrar" android:value="com.google.firebase.components.ComponentRegistrar" />
			<meta-data android:name="com.google.firebase.components:com.google.firebase.analytics.connector.internal.AnalyticsConnectorRegistrar" android:value="com.google.firebase.components.ComponentRegistrar" />
			<meta-data android:name="com.google.firebase.components:com.google.firebase.abt.component.AbtRegistrar" android:value="com.google.firebase.components.ComponentRegistrar" />
			<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar" />
		</service>
		<service android:directBootAware="true" android:exported="false" android:name="com.google.firebase.messaging.FirebaseMessagingService">
			<intent-filter android:priority="-500">
				<action android:name="com.google.firebase.MESSAGING_EVENT" />
			</intent-filter>
		</service>
		<service android:exported="false" android:name="com.google.android.datatransport.runtime.backends.TransportBackendDiscovery">
			<meta-data android:name="backend:com.google.android.datatransport.cct.CctBackendFactory" android:value="cct" />
		</service>
		<service android:exported="false" android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.JobInfoSchedulerService" android:permission="android.permission.BIND_JOB_SERVICE" />
		<receiver android:exported="false" android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.AlarmManagerSchedulerBroadcastReceiver" />
		<service android:directBootAware="true" android:exported="false" android:name="androidx.room.MultiInstanceInvalidationService" />
		<receiver android:enabled="true" android:exported="false" android:name="com.google.android.gms.measurement.AppMeasurementReceiver" />
		<service android:enabled="true" android:exported="false" android:name="com.google.android.gms.measurement.AppMeasurementService" />
		<service android:enabled="true" android:exported="false" android:name="com.google.android.gms.measurement.AppMeasurementJobService" android:permission="android.permission.BIND_JOB_SERVICE" />
		<receiver android:exported="true" android:name="com.google.firebase.iid.FirebaseInstanceIdReceiver" android:permission="com.google.android.c2dm.permission.SEND">
			<intent-filter>
				<action android:name="com.google.android.c2dm.intent.RECEIVE" />
			</intent-filter>
		</receiver>
		<provider android:authorities="com.ngc.fasttv.firebaseinitprovider" android:exported="false" android:initOrder="100" android:name="com.google.firebase.provider.FirebaseInitProvider" />
		<activity android:exported="false" android:name="com.google.android.gms.common.api.GoogleApiActivity" android:theme="@android:style/Theme.Translucent.NoTitleBar" />
		<meta-data android:name="com.google.android.gms.version" android:value="@integer/google_play_services_version" />
		<provider android:authorities="com.ngc.fasttv.lifecycle-process" android:exported="false" android:multiprocess="true" android:name="androidx.lifecycle.ProcessLifecycleOwnerInitializer" />
	</application>
</manifest>
