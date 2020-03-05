---
title: macOSKerberosSingleSignOnExtension 资源类型
description: 表示 macOS 设备的 Kerberos 类型单一登录扩展配置文件。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: caee357aa9a045caeb06aea15330892dfe80e631
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529689"
---
# <a name="macoskerberossinglesignonextension-resource-type"></a><span data-ttu-id="05980-103">macOSKerberosSingleSignOnExtension 资源类型</span><span class="sxs-lookup"><span data-stu-id="05980-103">macOSKerberosSingleSignOnExtension resource type</span></span>

<span data-ttu-id="05980-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="05980-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05980-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="05980-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05980-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="05980-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05980-107">表示 macOS 设备的 Kerberos 类型单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="05980-107">Represents a Kerberos-type Single Sign-On extension profile for macOS devices.</span></span>


<span data-ttu-id="05980-108">继承自[macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="05980-108">Inherits from [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="05980-109">属性</span><span class="sxs-lookup"><span data-stu-id="05980-109">Properties</span></span>
|<span data-ttu-id="05980-110">属性</span><span class="sxs-lookup"><span data-stu-id="05980-110">Property</span></span>|<span data-ttu-id="05980-111">类型</span><span class="sxs-lookup"><span data-stu-id="05980-111">Type</span></span>|<span data-ttu-id="05980-112">说明</span><span class="sxs-lookup"><span data-stu-id="05980-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05980-113">型</span><span class="sxs-lookup"><span data-stu-id="05980-113">realm</span></span>|<span data-ttu-id="05980-114">String</span><span class="sxs-lookup"><span data-stu-id="05980-114">String</span></span>|<span data-ttu-id="05980-115">获取或设置此配置文件的区分大小写的领域名称。</span><span class="sxs-lookup"><span data-stu-id="05980-115">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="05980-116">域</span><span class="sxs-lookup"><span data-stu-id="05980-116">domains</span></span>|<span data-ttu-id="05980-117">String 集合</span><span class="sxs-lookup"><span data-stu-id="05980-117">String collection</span></span>|<span data-ttu-id="05980-118">获取或设置应用程序扩展为其执行 SSO 的主机名或域名的列表。</span><span class="sxs-lookup"><span data-stu-id="05980-118">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="05980-119">blockAutomaticLogin</span><span class="sxs-lookup"><span data-stu-id="05980-119">blockAutomaticLogin</span></span>|<span data-ttu-id="05980-120">布尔</span><span class="sxs-lookup"><span data-stu-id="05980-120">Boolean</span></span>|<span data-ttu-id="05980-121">启用或禁用密钥链用法。</span><span class="sxs-lookup"><span data-stu-id="05980-121">Enables or disables Keychain usage.</span></span>|
|<span data-ttu-id="05980-122">cacheName</span><span class="sxs-lookup"><span data-stu-id="05980-122">cacheName</span></span>|<span data-ttu-id="05980-123">String</span><span class="sxs-lookup"><span data-stu-id="05980-123">String</span></span>|<span data-ttu-id="05980-124">获取或设置要用于此配置文件的 Kerberos 缓存的通用安全服务名称。</span><span class="sxs-lookup"><span data-stu-id="05980-124">Gets or sets the Generic Security Services name of the Kerberos cache to use for this profile.</span></span>|
|<span data-ttu-id="05980-125">credentialBundleIdAccessControlList</span><span class="sxs-lookup"><span data-stu-id="05980-125">credentialBundleIdAccessControlList</span></span>|<span data-ttu-id="05980-126">String 集合</span><span class="sxs-lookup"><span data-stu-id="05980-126">String collection</span></span>|<span data-ttu-id="05980-127">获取或设置允许访问 Kerberos 票证授予票证的应用捆绑包 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="05980-127">Gets or sets a list of app Bundle IDs allowed to access the Kerberos Ticket Granting Ticket.</span></span>|
|<span data-ttu-id="05980-128">domainRealms</span><span class="sxs-lookup"><span data-stu-id="05980-128">domainRealms</span></span>|<span data-ttu-id="05980-129">String 集合</span><span class="sxs-lookup"><span data-stu-id="05980-129">String collection</span></span>|<span data-ttu-id="05980-130">获取或设置自定义域领域映射的领域列表。</span><span class="sxs-lookup"><span data-stu-id="05980-130">Gets or sets a list of realms for custom domain-realm mapping.</span></span> <span data-ttu-id="05980-131">领域区分大小写。</span><span class="sxs-lookup"><span data-stu-id="05980-131">Realms are case sensitive.</span></span>|
|<span data-ttu-id="05980-132">isDefaultRealm</span><span class="sxs-lookup"><span data-stu-id="05980-132">isDefaultRealm</span></span>|<span data-ttu-id="05980-133">布尔</span><span class="sxs-lookup"><span data-stu-id="05980-133">Boolean</span></span>|<span data-ttu-id="05980-134">如果为 true，则将选择此配置文件的领域作为默认领域。</span><span class="sxs-lookup"><span data-stu-id="05980-134">When true, this profile's realm will be selected as the default.</span></span> <span data-ttu-id="05980-135">如果配置了多个 Kerberos 类型配置文件，则必须执行此步骤。</span><span class="sxs-lookup"><span data-stu-id="05980-135">Necessary if multiple Kerberos-type profiles are configured.</span></span>|
|<span data-ttu-id="05980-136">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="05980-136">passwordBlockModification</span></span>|<span data-ttu-id="05980-137">布尔</span><span class="sxs-lookup"><span data-stu-id="05980-137">Boolean</span></span>|<span data-ttu-id="05980-138">启用或禁用密码更改。</span><span class="sxs-lookup"><span data-stu-id="05980-138">Enables or disables password changes.</span></span>|
|<span data-ttu-id="05980-139">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="05980-139">passwordExpirationDays</span></span>|<span data-ttu-id="05980-140">Int32</span><span class="sxs-lookup"><span data-stu-id="05980-140">Int32</span></span>|<span data-ttu-id="05980-141">替代默认密码到期天数（天）。</span><span class="sxs-lookup"><span data-stu-id="05980-141">Overrides the default password expiration in days.</span></span> <span data-ttu-id="05980-142">对于大多数域，此值是自动计算的。</span><span class="sxs-lookup"><span data-stu-id="05980-142">For most domains, this value is calculated automatically.</span></span>|
|<span data-ttu-id="05980-143">passwordExpirationNotificationDays</span><span class="sxs-lookup"><span data-stu-id="05980-143">passwordExpirationNotificationDays</span></span>|<span data-ttu-id="05980-144">Int32</span><span class="sxs-lookup"><span data-stu-id="05980-144">Int32</span></span>|<span data-ttu-id="05980-145">获取或设置通知用户其密码将到期的天数（默认值为15）。</span><span class="sxs-lookup"><span data-stu-id="05980-145">Gets or sets the number of days until the user is notified that their password will expire (default is 15).</span></span>|
|<span data-ttu-id="05980-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="05980-146">userPrincipalName</span></span>|<span data-ttu-id="05980-147">String</span><span class="sxs-lookup"><span data-stu-id="05980-147">String</span></span>|<span data-ttu-id="05980-148">获取或设置要用于此配置文件的原理用户名。</span><span class="sxs-lookup"><span data-stu-id="05980-148">Gets or sets the principle user name to use for this profile.</span></span> <span data-ttu-id="05980-149">不需要包含领域名称。</span><span class="sxs-lookup"><span data-stu-id="05980-149">The realm name does not need to be included.</span></span>|
|<span data-ttu-id="05980-150">passwordRequireActiveDirectoryComplexity</span><span class="sxs-lookup"><span data-stu-id="05980-150">passwordRequireActiveDirectoryComplexity</span></span>|<span data-ttu-id="05980-151">布尔</span><span class="sxs-lookup"><span data-stu-id="05980-151">Boolean</span></span>|<span data-ttu-id="05980-152">启用或禁用密码是否必须符合 Active Directory 的复杂性要求。</span><span class="sxs-lookup"><span data-stu-id="05980-152">Enables or disables whether passwords must meet Active Directory's complexity requirements.</span></span>|
|<span data-ttu-id="05980-153">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="05980-153">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="05980-154">Int32</span><span class="sxs-lookup"><span data-stu-id="05980-154">Int32</span></span>|<span data-ttu-id="05980-155">获取或设置要阻止的以前密码的数目。</span><span class="sxs-lookup"><span data-stu-id="05980-155">Gets or sets the number of previous passwords to block.</span></span>|
|<span data-ttu-id="05980-156">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="05980-156">passwordMinimumLength</span></span>|<span data-ttu-id="05980-157">Int32</span><span class="sxs-lookup"><span data-stu-id="05980-157">Int32</span></span>|<span data-ttu-id="05980-158">获取或设置密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="05980-158">Gets or sets the minimum length of a password.</span></span>|
|<span data-ttu-id="05980-159">passwordMinimumAgeDays</span><span class="sxs-lookup"><span data-stu-id="05980-159">passwordMinimumAgeDays</span></span>|<span data-ttu-id="05980-160">Int32</span><span class="sxs-lookup"><span data-stu-id="05980-160">Int32</span></span>|<span data-ttu-id="05980-161">获取或设置用户可以再次更改密码之前的最小天数。</span><span class="sxs-lookup"><span data-stu-id="05980-161">Gets or sets the minimum number of days until a user can change their password again.</span></span>|
|<span data-ttu-id="05980-162">passwordRequirementsDescription</span><span class="sxs-lookup"><span data-stu-id="05980-162">passwordRequirementsDescription</span></span>|<span data-ttu-id="05980-163">String</span><span class="sxs-lookup"><span data-stu-id="05980-163">String</span></span>|<span data-ttu-id="05980-164">获取或设置密码复杂性要求的说明。</span><span class="sxs-lookup"><span data-stu-id="05980-164">Gets or sets a description of the password complexity requirements.</span></span>|
|<span data-ttu-id="05980-165">requireUserPresence</span><span class="sxs-lookup"><span data-stu-id="05980-165">requireUserPresence</span></span>|<span data-ttu-id="05980-166">布尔</span><span class="sxs-lookup"><span data-stu-id="05980-166">Boolean</span></span>|<span data-ttu-id="05980-167">获取或设置是否需要通过触摸 ID、面孔 ID 或密码进行身份验证以访问密钥链条目。</span><span class="sxs-lookup"><span data-stu-id="05980-167">Gets or sets whether to require authentication via Touch ID, Face ID, or a passcode to access the keychain entry.</span></span>|
|<span data-ttu-id="05980-168">activeDirectorySiteCode</span><span class="sxs-lookup"><span data-stu-id="05980-168">activeDirectorySiteCode</span></span>|<span data-ttu-id="05980-169">String</span><span class="sxs-lookup"><span data-stu-id="05980-169">String</span></span>|<span data-ttu-id="05980-170">获取或设置 Active Directory 站点。</span><span class="sxs-lookup"><span data-stu-id="05980-170">Gets or sets the Active Directory site.</span></span>|
|<span data-ttu-id="05980-171">passwordEnableLocalSync</span><span class="sxs-lookup"><span data-stu-id="05980-171">passwordEnableLocalSync</span></span>|<span data-ttu-id="05980-172">布尔</span><span class="sxs-lookup"><span data-stu-id="05980-172">Boolean</span></span>|<span data-ttu-id="05980-173">启用或禁用密码同步。</span><span class="sxs-lookup"><span data-stu-id="05980-173">Enables or disables password syncing.</span></span> <span data-ttu-id="05980-174">这不会影响使用 macOS 上的移动帐户登录的用户。</span><span class="sxs-lookup"><span data-stu-id="05980-174">This won't affect users logged in with a mobile account on macOS.</span></span>|
|<span data-ttu-id="05980-175">blockActiveDirectorySiteAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="05980-175">blockActiveDirectorySiteAutoDiscovery</span></span>|<span data-ttu-id="05980-176">布尔</span><span class="sxs-lookup"><span data-stu-id="05980-176">Boolean</span></span>|<span data-ttu-id="05980-177">启用或禁用 Kerberos 扩展是否可以自动确定其站点名称。</span><span class="sxs-lookup"><span data-stu-id="05980-177">Enables or disables whether the Kerberos extension can automatically determine its site name.</span></span>|
|<span data-ttu-id="05980-178">passwordChangeUrl</span><span class="sxs-lookup"><span data-stu-id="05980-178">passwordChangeUrl</span></span>|<span data-ttu-id="05980-179">String</span><span class="sxs-lookup"><span data-stu-id="05980-179">String</span></span>|<span data-ttu-id="05980-180">获取或设置用户启动密码更改时将发送到的 URL。</span><span class="sxs-lookup"><span data-stu-id="05980-180">Gets or sets the URL that the user will be sent to when they initiate a password change.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05980-181">关系</span><span class="sxs-lookup"><span data-stu-id="05980-181">Relationships</span></span>
<span data-ttu-id="05980-182">无</span><span class="sxs-lookup"><span data-stu-id="05980-182">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="05980-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="05980-183">JSON Representation</span></span>
<span data-ttu-id="05980-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05980-184">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSKerberosSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSKerberosSingleSignOnExtension",
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



