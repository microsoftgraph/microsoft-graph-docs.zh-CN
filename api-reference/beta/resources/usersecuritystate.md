---
title: userSecurityState 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
ms.openlocfilehash: f530ac1a657b4049c17bdcdd40f1dd5ea734f278
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045163"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="7b17d-104">userSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="7b17d-104">userSecurityState resource type</span></span>

 > <span data-ttu-id="7b17d-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7b17d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b17d-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7b17d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7b17d-107">包含状态信息的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="7b17d-107">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="7b17d-108">属性</span><span class="sxs-lookup"><span data-stu-id="7b17d-108">Properties</span></span>

| <span data-ttu-id="7b17d-109">属性</span><span class="sxs-lookup"><span data-stu-id="7b17d-109">Property</span></span>   | <span data-ttu-id="7b17d-110">类型</span><span class="sxs-lookup"><span data-stu-id="7b17d-110">Type</span></span> |<span data-ttu-id="7b17d-111">说明</span><span class="sxs-lookup"><span data-stu-id="7b17d-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b17d-112">aadUserId</span><span class="sxs-lookup"><span data-stu-id="7b17d-112">aadUserId</span></span>|<span data-ttu-id="7b17d-113">字符串</span><span class="sxs-lookup"><span data-stu-id="7b17d-113">String</span></span>|<span data-ttu-id="7b17d-114">AAD 用户对象标识符 (GUID)-表示物理/多 account 用户实体。</span><span class="sxs-lookup"><span data-stu-id="7b17d-114">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="7b17d-115">accountName</span><span class="sxs-lookup"><span data-stu-id="7b17d-115">accountName</span></span>|<span data-ttu-id="7b17d-116">字符串</span><span class="sxs-lookup"><span data-stu-id="7b17d-116">String</span></span>|<span data-ttu-id="7b17d-117">（没有 Active Directory 域和 DNS 域） 的用户帐户的帐户名 (也称为`mailNickName`)。</span><span class="sxs-lookup"><span data-stu-id="7b17d-117">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="7b17d-118">domainName</span><span class="sxs-lookup"><span data-stu-id="7b17d-118">domainName</span></span>|<span data-ttu-id="7b17d-119">String</span><span class="sxs-lookup"><span data-stu-id="7b17d-119">String</span></span>|<span data-ttu-id="7b17d-120">NetBIOS/Active Directory 域的用户帐户 （即域 \ 帐户格式）。</span><span class="sxs-lookup"><span data-stu-id="7b17d-120">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="7b17d-121">emailRole</span><span class="sxs-lookup"><span data-stu-id="7b17d-121">emailRole</span></span>|<span data-ttu-id="7b17d-122">emailRole</span><span class="sxs-lookup"><span data-stu-id="7b17d-122">emailRole</span></span>|<span data-ttu-id="7b17d-123">电子邮件相关的通知的用户帐户的电子邮件角色。</span><span class="sxs-lookup"><span data-stu-id="7b17d-123">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="7b17d-124">可取值为：`unknown`、`sender`、`recipient`。</span><span class="sxs-lookup"><span data-stu-id="7b17d-124">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="7b17d-125">isVpn</span><span class="sxs-lookup"><span data-stu-id="7b17d-125">isVpn</span></span>|<span data-ttu-id="7b17d-126">布尔</span><span class="sxs-lookup"><span data-stu-id="7b17d-126">Boolean</span></span>|<span data-ttu-id="7b17d-127">指示用户是否可以通过 VPN 登录。</span><span class="sxs-lookup"><span data-stu-id="7b17d-127">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="7b17d-128">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="7b17d-128">logonDateTime</span></span>|<span data-ttu-id="7b17d-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b17d-129">DateTimeOffset</span></span>|<span data-ttu-id="7b17d-130">在登录所发生的时间。</span><span class="sxs-lookup"><span data-stu-id="7b17d-130">Time at which the sign-in occurred.</span></span> <span data-ttu-id="7b17d-131">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="7b17d-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7b17d-132">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="7b17d-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="7b17d-133">logonId</span><span class="sxs-lookup"><span data-stu-id="7b17d-133">logonId</span></span>|<span data-ttu-id="7b17d-134">字符串</span><span class="sxs-lookup"><span data-stu-id="7b17d-134">String</span></span>|<span data-ttu-id="7b17d-135">用户登录 id。</span><span class="sxs-lookup"><span data-stu-id="7b17d-135">User sign-in ID.</span></span>|
|<span data-ttu-id="7b17d-136">logonIp</span><span class="sxs-lookup"><span data-stu-id="7b17d-136">logonIp</span></span>|<span data-ttu-id="7b17d-137">字符串</span><span class="sxs-lookup"><span data-stu-id="7b17d-137">String</span></span>|<span data-ttu-id="7b17d-138">登录请求源自的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="7b17d-138">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="7b17d-139">logonLocation</span><span class="sxs-lookup"><span data-stu-id="7b17d-139">logonLocation</span></span>|<span data-ttu-id="7b17d-140">字符串</span><span class="sxs-lookup"><span data-stu-id="7b17d-140">String</span></span>|<span data-ttu-id="7b17d-141">此用户相关联的用户登录事件 （由 IP 地址映射） 位置。</span><span class="sxs-lookup"><span data-stu-id="7b17d-141">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="7b17d-142">logonType</span><span class="sxs-lookup"><span data-stu-id="7b17d-142">logonType</span></span>|<span data-ttu-id="7b17d-143">logonType</span><span class="sxs-lookup"><span data-stu-id="7b17d-143">logonType</span></span>|<span data-ttu-id="7b17d-144">用户登录的方法。</span><span class="sxs-lookup"><span data-stu-id="7b17d-144">Method of user sign in.</span></span> <span data-ttu-id="7b17d-145">可取值为：`unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。</span><span class="sxs-lookup"><span data-stu-id="7b17d-145">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="7b17d-146">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="7b17d-146">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="7b17d-147">字符串</span><span class="sxs-lookup"><span data-stu-id="7b17d-147">String</span></span>|<span data-ttu-id="7b17d-148">Active Directory （本地） 安全标识符 (SID) 的用户。</span><span class="sxs-lookup"><span data-stu-id="7b17d-148">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="7b17d-149">riskScore</span><span class="sxs-lookup"><span data-stu-id="7b17d-149">riskScore</span></span>|<span data-ttu-id="7b17d-150">字符串</span><span class="sxs-lookup"><span data-stu-id="7b17d-150">String</span></span>|<span data-ttu-id="7b17d-151">带有提供程序生成/计算风险的用户帐户的分数。</span><span class="sxs-lookup"><span data-stu-id="7b17d-151">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="7b17d-152">建议值的范围为 0-1，这相当于百分比。</span><span class="sxs-lookup"><span data-stu-id="7b17d-152">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="7b17d-153">userAccountType</span><span class="sxs-lookup"><span data-stu-id="7b17d-153">userAccountType</span></span>|<span data-ttu-id="7b17d-154">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="7b17d-154">userAccountSecurityType</span></span>|<span data-ttu-id="7b17d-155">用户帐户类型 （组成员身份），每 Windows 定义。</span><span class="sxs-lookup"><span data-stu-id="7b17d-155">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="7b17d-156">可取值为：`unknown`、`standard`、`power`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="7b17d-156">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="7b17d-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7b17d-157">userPrincipalName</span></span>|<span data-ttu-id="7b17d-158">字符串</span><span class="sxs-lookup"><span data-stu-id="7b17d-158">String</span></span>|<span data-ttu-id="7b17d-159">用户登录名-internet 格式: （用户帐户名） @ （用户帐户 DNS 域名）。</span><span class="sxs-lookup"><span data-stu-id="7b17d-159">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b17d-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7b17d-160">JSON representation</span></span>

<span data-ttu-id="7b17d-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b17d-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSecurityState"
}-->

```json
{
  "aadUserId": "String",
  "accountName": "String",
  "domainName": "String",
  "emailRole": "@odata.type: microsoft.graph.emailRole",
  "isVpn": true,
  "logonDateTime": "String (timestamp)",
  "logonId": "String",
  "logonIp": "String",
  "logonLocation": "String",
  "logonType": "@odata.type: microsoft.graph.logonType",
  "onPremisesSecurityIdentifier": "String",
  "riskScore": "String",
  "userAccountType": "@odata.type: microsoft.graph.userAccountSecurityType",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
