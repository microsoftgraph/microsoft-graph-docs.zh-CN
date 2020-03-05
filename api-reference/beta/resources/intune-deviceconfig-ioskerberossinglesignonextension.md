---
title: iosKerberosSingleSignOnExtension 资源类型
description: 表示 iOS 设备的 Kerberos 类型单一登录扩展配置文件。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e4d20aac5a72936c189a792ba4f3544ed9e96eb9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526337"
---
# <a name="ioskerberossinglesignonextension-resource-type"></a><span data-ttu-id="5f592-103">iosKerberosSingleSignOnExtension 资源类型</span><span class="sxs-lookup"><span data-stu-id="5f592-103">iosKerberosSingleSignOnExtension resource type</span></span>

<span data-ttu-id="5f592-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5f592-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5f592-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5f592-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f592-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5f592-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f592-107">表示 iOS 设备的 Kerberos 类型单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="5f592-107">Represents a Kerberos-type Single Sign-On extension profile for iOS devices.</span></span>


<span data-ttu-id="5f592-108">继承自[iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="5f592-108">Inherits from [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5f592-109">属性</span><span class="sxs-lookup"><span data-stu-id="5f592-109">Properties</span></span>
|<span data-ttu-id="5f592-110">属性</span><span class="sxs-lookup"><span data-stu-id="5f592-110">Property</span></span>|<span data-ttu-id="5f592-111">类型</span><span class="sxs-lookup"><span data-stu-id="5f592-111">Type</span></span>|<span data-ttu-id="5f592-112">说明</span><span class="sxs-lookup"><span data-stu-id="5f592-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f592-113">型</span><span class="sxs-lookup"><span data-stu-id="5f592-113">realm</span></span>|<span data-ttu-id="5f592-114">String</span><span class="sxs-lookup"><span data-stu-id="5f592-114">String</span></span>|<span data-ttu-id="5f592-115">获取或设置此配置文件的区分大小写的领域名称。</span><span class="sxs-lookup"><span data-stu-id="5f592-115">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="5f592-116">域</span><span class="sxs-lookup"><span data-stu-id="5f592-116">domains</span></span>|<span data-ttu-id="5f592-117">String 集合</span><span class="sxs-lookup"><span data-stu-id="5f592-117">String collection</span></span>|<span data-ttu-id="5f592-118">获取或设置应用程序扩展为其执行 SSO 的主机名或域名的列表。</span><span class="sxs-lookup"><span data-stu-id="5f592-118">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="5f592-119">blockAutomaticLogin</span><span class="sxs-lookup"><span data-stu-id="5f592-119">blockAutomaticLogin</span></span>|<span data-ttu-id="5f592-120">布尔</span><span class="sxs-lookup"><span data-stu-id="5f592-120">Boolean</span></span>|<span data-ttu-id="5f592-121">启用或禁用密钥链用法。</span><span class="sxs-lookup"><span data-stu-id="5f592-121">Enables or disables Keychain usage.</span></span>|
|<span data-ttu-id="5f592-122">cacheName</span><span class="sxs-lookup"><span data-stu-id="5f592-122">cacheName</span></span>|<span data-ttu-id="5f592-123">String</span><span class="sxs-lookup"><span data-stu-id="5f592-123">String</span></span>|<span data-ttu-id="5f592-124">获取或设置要用于此配置文件的 Kerberos 缓存的通用安全服务名称。</span><span class="sxs-lookup"><span data-stu-id="5f592-124">Gets or sets the Generic Security Services name of the Kerberos cache to use for this profile.</span></span>|
|<span data-ttu-id="5f592-125">credentialBundleIdAccessControlList</span><span class="sxs-lookup"><span data-stu-id="5f592-125">credentialBundleIdAccessControlList</span></span>|<span data-ttu-id="5f592-126">String 集合</span><span class="sxs-lookup"><span data-stu-id="5f592-126">String collection</span></span>|<span data-ttu-id="5f592-127">获取或设置允许访问 Kerberos 票证授予票证的应用捆绑包 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="5f592-127">Gets or sets a list of app Bundle IDs allowed to access the Kerberos Ticket Granting Ticket.</span></span>|
|<span data-ttu-id="5f592-128">domainRealms</span><span class="sxs-lookup"><span data-stu-id="5f592-128">domainRealms</span></span>|<span data-ttu-id="5f592-129">String 集合</span><span class="sxs-lookup"><span data-stu-id="5f592-129">String collection</span></span>|<span data-ttu-id="5f592-130">获取或设置自定义域领域映射的领域列表。</span><span class="sxs-lookup"><span data-stu-id="5f592-130">Gets or sets a list of realms for custom domain-realm mapping.</span></span> <span data-ttu-id="5f592-131">领域区分大小写。</span><span class="sxs-lookup"><span data-stu-id="5f592-131">Realms are case sensitive.</span></span>|
|<span data-ttu-id="5f592-132">isDefaultRealm</span><span class="sxs-lookup"><span data-stu-id="5f592-132">isDefaultRealm</span></span>|<span data-ttu-id="5f592-133">布尔</span><span class="sxs-lookup"><span data-stu-id="5f592-133">Boolean</span></span>|<span data-ttu-id="5f592-134">如果为 true，则将选择此配置文件的领域作为默认领域。</span><span class="sxs-lookup"><span data-stu-id="5f592-134">When true, this profile's realm will be selected as the default.</span></span> <span data-ttu-id="5f592-135">如果配置了多个 Kerberos 类型配置文件，则必须执行此步骤。</span><span class="sxs-lookup"><span data-stu-id="5f592-135">Necessary if multiple Kerberos-type profiles are configured.</span></span>|
|<span data-ttu-id="5f592-136">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="5f592-136">passwordBlockModification</span></span>|<span data-ttu-id="5f592-137">布尔</span><span class="sxs-lookup"><span data-stu-id="5f592-137">Boolean</span></span>|<span data-ttu-id="5f592-138">启用或禁用密码更改。</span><span class="sxs-lookup"><span data-stu-id="5f592-138">Enables or disables password changes.</span></span>|
|<span data-ttu-id="5f592-139">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5f592-139">passwordExpirationDays</span></span>|<span data-ttu-id="5f592-140">Int32</span><span class="sxs-lookup"><span data-stu-id="5f592-140">Int32</span></span>|<span data-ttu-id="5f592-141">替代默认密码到期天数（天）。</span><span class="sxs-lookup"><span data-stu-id="5f592-141">Overrides the default password expiration in days.</span></span> <span data-ttu-id="5f592-142">对于大多数域，此值是自动计算的。</span><span class="sxs-lookup"><span data-stu-id="5f592-142">For most domains, this value is calculated automatically.</span></span>|
|<span data-ttu-id="5f592-143">passwordExpirationNotificationDays</span><span class="sxs-lookup"><span data-stu-id="5f592-143">passwordExpirationNotificationDays</span></span>|<span data-ttu-id="5f592-144">Int32</span><span class="sxs-lookup"><span data-stu-id="5f592-144">Int32</span></span>|<span data-ttu-id="5f592-145">获取或设置通知用户其密码将到期的天数（默认值为15）。</span><span class="sxs-lookup"><span data-stu-id="5f592-145">Gets or sets the number of days until the user is notified that their password will expire (default is 15).</span></span>|
|<span data-ttu-id="5f592-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5f592-146">userPrincipalName</span></span>|<span data-ttu-id="5f592-147">String</span><span class="sxs-lookup"><span data-stu-id="5f592-147">String</span></span>|<span data-ttu-id="5f592-148">获取或设置要用于此配置文件的原理用户名。</span><span class="sxs-lookup"><span data-stu-id="5f592-148">Gets or sets the principle user name to use for this profile.</span></span> <span data-ttu-id="5f592-149">不需要包含领域名称。</span><span class="sxs-lookup"><span data-stu-id="5f592-149">The realm name does not need to be included.</span></span>|
|<span data-ttu-id="5f592-150">passwordRequireActiveDirectoryComplexity</span><span class="sxs-lookup"><span data-stu-id="5f592-150">passwordRequireActiveDirectoryComplexity</span></span>|<span data-ttu-id="5f592-151">布尔</span><span class="sxs-lookup"><span data-stu-id="5f592-151">Boolean</span></span>|<span data-ttu-id="5f592-152">启用或禁用密码是否必须符合 Active Directory 的复杂性要求。</span><span class="sxs-lookup"><span data-stu-id="5f592-152">Enables or disables whether passwords must meet Active Directory's complexity requirements.</span></span>|
|<span data-ttu-id="5f592-153">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="5f592-153">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="5f592-154">Int32</span><span class="sxs-lookup"><span data-stu-id="5f592-154">Int32</span></span>|<span data-ttu-id="5f592-155">获取或设置要阻止的以前密码的数目。</span><span class="sxs-lookup"><span data-stu-id="5f592-155">Gets or sets the number of previous passwords to block.</span></span>|
|<span data-ttu-id="5f592-156">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5f592-156">passwordMinimumLength</span></span>|<span data-ttu-id="5f592-157">Int32</span><span class="sxs-lookup"><span data-stu-id="5f592-157">Int32</span></span>|<span data-ttu-id="5f592-158">获取或设置密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="5f592-158">Gets or sets the minimum length of a password.</span></span>|
|<span data-ttu-id="5f592-159">passwordMinimumAgeDays</span><span class="sxs-lookup"><span data-stu-id="5f592-159">passwordMinimumAgeDays</span></span>|<span data-ttu-id="5f592-160">Int32</span><span class="sxs-lookup"><span data-stu-id="5f592-160">Int32</span></span>|<span data-ttu-id="5f592-161">获取或设置用户可以再次更改密码之前的最小天数。</span><span class="sxs-lookup"><span data-stu-id="5f592-161">Gets or sets the minimum number of days until a user can change their password again.</span></span>|
|<span data-ttu-id="5f592-162">passwordRequirementsDescription</span><span class="sxs-lookup"><span data-stu-id="5f592-162">passwordRequirementsDescription</span></span>|<span data-ttu-id="5f592-163">String</span><span class="sxs-lookup"><span data-stu-id="5f592-163">String</span></span>|<span data-ttu-id="5f592-164">获取或设置密码复杂性要求的说明。</span><span class="sxs-lookup"><span data-stu-id="5f592-164">Gets or sets a description of the password complexity requirements.</span></span>|
|<span data-ttu-id="5f592-165">requireUserPresence</span><span class="sxs-lookup"><span data-stu-id="5f592-165">requireUserPresence</span></span>|<span data-ttu-id="5f592-166">布尔</span><span class="sxs-lookup"><span data-stu-id="5f592-166">Boolean</span></span>|<span data-ttu-id="5f592-167">获取或设置是否需要通过触摸 ID、面孔 ID 或密码进行身份验证以访问密钥链条目。</span><span class="sxs-lookup"><span data-stu-id="5f592-167">Gets or sets whether to require authentication via Touch ID, Face ID, or a passcode to access the keychain entry.</span></span>|
|<span data-ttu-id="5f592-168">activeDirectorySiteCode</span><span class="sxs-lookup"><span data-stu-id="5f592-168">activeDirectorySiteCode</span></span>|<span data-ttu-id="5f592-169">String</span><span class="sxs-lookup"><span data-stu-id="5f592-169">String</span></span>|<span data-ttu-id="5f592-170">获取或设置 Active Directory 站点。</span><span class="sxs-lookup"><span data-stu-id="5f592-170">Gets or sets the Active Directory site.</span></span>|
|<span data-ttu-id="5f592-171">passwordEnableLocalSync</span><span class="sxs-lookup"><span data-stu-id="5f592-171">passwordEnableLocalSync</span></span>|<span data-ttu-id="5f592-172">布尔</span><span class="sxs-lookup"><span data-stu-id="5f592-172">Boolean</span></span>|<span data-ttu-id="5f592-173">启用或禁用密码同步。</span><span class="sxs-lookup"><span data-stu-id="5f592-173">Enables or disables password syncing.</span></span> <span data-ttu-id="5f592-174">这不会影响使用 macOS 上的移动帐户登录的用户。</span><span class="sxs-lookup"><span data-stu-id="5f592-174">This won't affect users logged in with a mobile account on macOS.</span></span>|
|<span data-ttu-id="5f592-175">blockActiveDirectorySiteAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="5f592-175">blockActiveDirectorySiteAutoDiscovery</span></span>|<span data-ttu-id="5f592-176">布尔</span><span class="sxs-lookup"><span data-stu-id="5f592-176">Boolean</span></span>|<span data-ttu-id="5f592-177">启用或禁用 Kerberos 扩展是否可以自动确定其站点名称。</span><span class="sxs-lookup"><span data-stu-id="5f592-177">Enables or disables whether the Kerberos extension can automatically determine its site name.</span></span>|
|<span data-ttu-id="5f592-178">passwordChangeUrl</span><span class="sxs-lookup"><span data-stu-id="5f592-178">passwordChangeUrl</span></span>|<span data-ttu-id="5f592-179">String</span><span class="sxs-lookup"><span data-stu-id="5f592-179">String</span></span>|<span data-ttu-id="5f592-180">获取或设置用户启动密码更改时将发送到的 URL。</span><span class="sxs-lookup"><span data-stu-id="5f592-180">Gets or sets the URL that the user will be sent to when they initiate a password change.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f592-181">关系</span><span class="sxs-lookup"><span data-stu-id="5f592-181">Relationships</span></span>
<span data-ttu-id="5f592-182">无</span><span class="sxs-lookup"><span data-stu-id="5f592-182">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f592-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5f592-183">JSON Representation</span></span>
<span data-ttu-id="5f592-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f592-184">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosKerberosSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosKerberosSingleSignOnExtension",
  "realm": "String",
  "domains": [
    "String"
  ],
  "blockAutomaticLogin": true,
  "cacheName": "String",
  "credentialBundleIdAccessControlList": [
    "String"
  ],
  "domainRealms": [
    "String"
  ],
  "isDefaultRealm": true,
  "passwordBlockModification": true,
  "passwordExpirationDays": 1024,
  "passwordExpirationNotificationDays": 1024,
  "userPrincipalName": "String",
  "passwordRequireActiveDirectoryComplexity": true,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinimumAgeDays": 1024,
  "passwordRequirementsDescription": "String",
  "requireUserPresence": true,
  "activeDirectorySiteCode": "String",
  "passwordEnableLocalSync": true,
  "blockActiveDirectorySiteAutoDiscovery": true,
  "passwordChangeUrl": "String"
}
```



