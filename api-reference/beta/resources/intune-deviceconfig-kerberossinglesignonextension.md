---
title: kerberosSingleSignOnExtension 资源类型
description: 表示 Kerberos 类型的单一登录扩展配置文件。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 443ccdeac8d2249714c0cdad4af3748482acda3a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37200017"
---
# <a name="kerberossinglesignonextension-resource-type"></a><span data-ttu-id="e3e32-103">kerberosSingleSignOnExtension 资源类型</span><span class="sxs-lookup"><span data-stu-id="e3e32-103">kerberosSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="e3e32-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e3e32-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3e32-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e3e32-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3e32-106">表示 Kerberos 类型的单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="e3e32-106">Represents a Kerberos-type Single Sign-On extension profile.</span></span>


<span data-ttu-id="e3e32-107">继承自[singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="e3e32-107">Inherits from [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e3e32-108">属性</span><span class="sxs-lookup"><span data-stu-id="e3e32-108">Properties</span></span>
|<span data-ttu-id="e3e32-109">属性</span><span class="sxs-lookup"><span data-stu-id="e3e32-109">Property</span></span>|<span data-ttu-id="e3e32-110">类型</span><span class="sxs-lookup"><span data-stu-id="e3e32-110">Type</span></span>|<span data-ttu-id="e3e32-111">说明</span><span class="sxs-lookup"><span data-stu-id="e3e32-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3e32-112">型</span><span class="sxs-lookup"><span data-stu-id="e3e32-112">realm</span></span>|<span data-ttu-id="e3e32-113">String</span><span class="sxs-lookup"><span data-stu-id="e3e32-113">String</span></span>|<span data-ttu-id="e3e32-114">获取或设置此配置文件的区分大小写的领域名称。</span><span class="sxs-lookup"><span data-stu-id="e3e32-114">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="e3e32-115">域</span><span class="sxs-lookup"><span data-stu-id="e3e32-115">domains</span></span>|<span data-ttu-id="e3e32-116">String collection</span><span class="sxs-lookup"><span data-stu-id="e3e32-116">String collection</span></span>|<span data-ttu-id="e3e32-117">获取或设置应用程序扩展为其执行 SSO 的主机名或域名的列表。</span><span class="sxs-lookup"><span data-stu-id="e3e32-117">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="e3e32-118">blockAutomaticLogin</span><span class="sxs-lookup"><span data-stu-id="e3e32-118">blockAutomaticLogin</span></span>|<span data-ttu-id="e3e32-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3e32-119">Boolean</span></span>|<span data-ttu-id="e3e32-120">启用或禁用密钥链用法。</span><span class="sxs-lookup"><span data-stu-id="e3e32-120">Enables or disables Keychain usage.</span></span>|
|<span data-ttu-id="e3e32-121">cacheName</span><span class="sxs-lookup"><span data-stu-id="e3e32-121">cacheName</span></span>|<span data-ttu-id="e3e32-122">String</span><span class="sxs-lookup"><span data-stu-id="e3e32-122">String</span></span>|<span data-ttu-id="e3e32-123">获取或设置要用于此配置文件的 Kerberos 缓存的通用安全服务名称。</span><span class="sxs-lookup"><span data-stu-id="e3e32-123">Gets or sets the Generic Security Services name of the Kerberos cache to use for this profile.</span></span>|
|<span data-ttu-id="e3e32-124">credentialBundleIdAccessControlList</span><span class="sxs-lookup"><span data-stu-id="e3e32-124">credentialBundleIdAccessControlList</span></span>|<span data-ttu-id="e3e32-125">String collection</span><span class="sxs-lookup"><span data-stu-id="e3e32-125">String collection</span></span>|<span data-ttu-id="e3e32-126">获取或设置允许访问 Kerberos 票证授予票证的应用捆绑包 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="e3e32-126">Gets or sets a list of app Bundle IDs allowed to access the Kerberos Ticket Granting Ticket.</span></span>|
|<span data-ttu-id="e3e32-127">domainRealms</span><span class="sxs-lookup"><span data-stu-id="e3e32-127">domainRealms</span></span>|<span data-ttu-id="e3e32-128">String collection</span><span class="sxs-lookup"><span data-stu-id="e3e32-128">String collection</span></span>|<span data-ttu-id="e3e32-129">获取或设置自定义域领域映射的领域列表。</span><span class="sxs-lookup"><span data-stu-id="e3e32-129">Gets or sets a list of realms for custom domain-realm mapping.</span></span> <span data-ttu-id="e3e32-130">领域区分大小写。</span><span class="sxs-lookup"><span data-stu-id="e3e32-130">Realms are case sensitive.</span></span>|
|<span data-ttu-id="e3e32-131">isDefaultRealm</span><span class="sxs-lookup"><span data-stu-id="e3e32-131">isDefaultRealm</span></span>|<span data-ttu-id="e3e32-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3e32-132">Boolean</span></span>|<span data-ttu-id="e3e32-133">如果为 true，则将选择此配置文件的领域作为默认领域。</span><span class="sxs-lookup"><span data-stu-id="e3e32-133">When true, this profile's realm will be selected as the default.</span></span> <span data-ttu-id="e3e32-134">如果配置了多个 Kerberos 类型配置文件，则必须执行此步骤。</span><span class="sxs-lookup"><span data-stu-id="e3e32-134">Necessary if multiple Kerberos-type profiles are configured.</span></span>|
|<span data-ttu-id="e3e32-135">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="e3e32-135">passwordBlockModification</span></span>|<span data-ttu-id="e3e32-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3e32-136">Boolean</span></span>|<span data-ttu-id="e3e32-137">启用或禁用密码更改。</span><span class="sxs-lookup"><span data-stu-id="e3e32-137">Enables or disables password changes.</span></span>|
|<span data-ttu-id="e3e32-138">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e3e32-138">passwordExpirationDays</span></span>|<span data-ttu-id="e3e32-139">Int32</span><span class="sxs-lookup"><span data-stu-id="e3e32-139">Int32</span></span>|<span data-ttu-id="e3e32-140">替代默认密码到期天数（天）。</span><span class="sxs-lookup"><span data-stu-id="e3e32-140">Overrides the default password expiration in days.</span></span> <span data-ttu-id="e3e32-141">对于大多数域，此值是自动计算的。</span><span class="sxs-lookup"><span data-stu-id="e3e32-141">For most domains, this value is calculated automatically.</span></span>|
|<span data-ttu-id="e3e32-142">passwordExpirationNotificationDays</span><span class="sxs-lookup"><span data-stu-id="e3e32-142">passwordExpirationNotificationDays</span></span>|<span data-ttu-id="e3e32-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e3e32-143">Int32</span></span>|<span data-ttu-id="e3e32-144">获取或设置通知用户其密码将到期的天数（默认值为15）。</span><span class="sxs-lookup"><span data-stu-id="e3e32-144">Gets or sets the number of days until the user is notified that their password will expire (default is 15).</span></span>|
|<span data-ttu-id="e3e32-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e3e32-145">userPrincipalName</span></span>|<span data-ttu-id="e3e32-146">String</span><span class="sxs-lookup"><span data-stu-id="e3e32-146">String</span></span>|<span data-ttu-id="e3e32-147">获取或设置要用于此配置文件的原理用户名。</span><span class="sxs-lookup"><span data-stu-id="e3e32-147">Gets or sets the principle user name to use for this profile.</span></span> <span data-ttu-id="e3e32-148">不需要包含领域名称。</span><span class="sxs-lookup"><span data-stu-id="e3e32-148">The realm name does not need to be included.</span></span>|
|<span data-ttu-id="e3e32-149">passwordRequireActiveDirectoryComplexity</span><span class="sxs-lookup"><span data-stu-id="e3e32-149">passwordRequireActiveDirectoryComplexity</span></span>|<span data-ttu-id="e3e32-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3e32-150">Boolean</span></span>|<span data-ttu-id="e3e32-151">启用或禁用密码是否必须符合 Active Directory 的复杂性要求。</span><span class="sxs-lookup"><span data-stu-id="e3e32-151">Enables or disables whether passwords must meet Active Directory's complexity requirements.</span></span>|
|<span data-ttu-id="e3e32-152">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e3e32-152">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e3e32-153">Int32</span><span class="sxs-lookup"><span data-stu-id="e3e32-153">Int32</span></span>|<span data-ttu-id="e3e32-154">获取或设置要阻止的以前密码的数目。</span><span class="sxs-lookup"><span data-stu-id="e3e32-154">Gets or sets the number of previous passwords to block.</span></span>|
|<span data-ttu-id="e3e32-155">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e3e32-155">passwordMinimumLength</span></span>|<span data-ttu-id="e3e32-156">Int32</span><span class="sxs-lookup"><span data-stu-id="e3e32-156">Int32</span></span>|<span data-ttu-id="e3e32-157">获取或设置密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="e3e32-157">Gets or sets the minimum length of a password.</span></span>|
|<span data-ttu-id="e3e32-158">passwordMinimumAgeDays</span><span class="sxs-lookup"><span data-stu-id="e3e32-158">passwordMinimumAgeDays</span></span>|<span data-ttu-id="e3e32-159">Int32</span><span class="sxs-lookup"><span data-stu-id="e3e32-159">Int32</span></span>|<span data-ttu-id="e3e32-160">获取或设置用户可以再次更改密码之前的最小天数。</span><span class="sxs-lookup"><span data-stu-id="e3e32-160">Gets or sets the minimum number of days until a user can change their password again.</span></span>|
|<span data-ttu-id="e3e32-161">passwordRequirementsDescription</span><span class="sxs-lookup"><span data-stu-id="e3e32-161">passwordRequirementsDescription</span></span>|<span data-ttu-id="e3e32-162">String</span><span class="sxs-lookup"><span data-stu-id="e3e32-162">String</span></span>|<span data-ttu-id="e3e32-163">获取或设置密码复杂性要求的说明。</span><span class="sxs-lookup"><span data-stu-id="e3e32-163">Gets or sets a description of the password complexity requirements.</span></span>|
|<span data-ttu-id="e3e32-164">requireUserPresence</span><span class="sxs-lookup"><span data-stu-id="e3e32-164">requireUserPresence</span></span>|<span data-ttu-id="e3e32-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3e32-165">Boolean</span></span>|<span data-ttu-id="e3e32-166">获取或设置是否需要通过触摸 ID、面孔 ID 或密码进行身份验证以访问密钥链条目。</span><span class="sxs-lookup"><span data-stu-id="e3e32-166">Gets or sets whether to require authentication via Touch ID, Face ID, or a passcode to access the keychain entry.</span></span>|
|<span data-ttu-id="e3e32-167">activeDirectorySiteCode</span><span class="sxs-lookup"><span data-stu-id="e3e32-167">activeDirectorySiteCode</span></span>|<span data-ttu-id="e3e32-168">String</span><span class="sxs-lookup"><span data-stu-id="e3e32-168">String</span></span>|<span data-ttu-id="e3e32-169">获取或设置 Active Directory 站点。</span><span class="sxs-lookup"><span data-stu-id="e3e32-169">Gets or sets the Active Directory site.</span></span>|
|<span data-ttu-id="e3e32-170">passwordEnableLocalSync</span><span class="sxs-lookup"><span data-stu-id="e3e32-170">passwordEnableLocalSync</span></span>|<span data-ttu-id="e3e32-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3e32-171">Boolean</span></span>|<span data-ttu-id="e3e32-172">启用或禁用密码同步。</span><span class="sxs-lookup"><span data-stu-id="e3e32-172">Enables or disables password syncing.</span></span> <span data-ttu-id="e3e32-173">这不会影响使用 macOS 上的移动帐户登录的用户。</span><span class="sxs-lookup"><span data-stu-id="e3e32-173">This won't affect users logged in with a mobile account on macOS.</span></span>|
|<span data-ttu-id="e3e32-174">blockActiveDirectorySiteAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="e3e32-174">blockActiveDirectorySiteAutoDiscovery</span></span>|<span data-ttu-id="e3e32-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3e32-175">Boolean</span></span>|<span data-ttu-id="e3e32-176">启用或禁用 Kerberos 扩展是否可以自动确定其站点名称。</span><span class="sxs-lookup"><span data-stu-id="e3e32-176">Enables or disables whether the Kerberos extension can automatically determine its site name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3e32-177">关系</span><span class="sxs-lookup"><span data-stu-id="e3e32-177">Relationships</span></span>
<span data-ttu-id="e3e32-178">无</span><span class="sxs-lookup"><span data-stu-id="e3e32-178">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3e32-179">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e3e32-179">JSON Representation</span></span>
<span data-ttu-id="e3e32-180">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3e32-180">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.kerberosSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.kerberosSingleSignOnExtension",
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
  "blockActiveDirectorySiteAutoDiscovery": true
}
```



