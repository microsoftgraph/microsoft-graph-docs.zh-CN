---
title: userSecurityState 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 62a54a996d7fe9c892da797cee352a57d0782035
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517237"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="8ec95-104">userSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="8ec95-104">userSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ec95-105">包含状态信息的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="8ec95-105">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="8ec95-106">属性</span><span class="sxs-lookup"><span data-stu-id="8ec95-106">Properties</span></span>

| <span data-ttu-id="8ec95-107">属性</span><span class="sxs-lookup"><span data-stu-id="8ec95-107">Property</span></span>   | <span data-ttu-id="8ec95-108">类型</span><span class="sxs-lookup"><span data-stu-id="8ec95-108">Type</span></span> |<span data-ttu-id="8ec95-109">说明</span><span class="sxs-lookup"><span data-stu-id="8ec95-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ec95-110">aadUserId</span><span class="sxs-lookup"><span data-stu-id="8ec95-110">aadUserId</span></span>|<span data-ttu-id="8ec95-111">String</span><span class="sxs-lookup"><span data-stu-id="8ec95-111">String</span></span>|<span data-ttu-id="8ec95-112">AAD 用户对象标识符 (GUID)-表示物理/多 account 用户实体。</span><span class="sxs-lookup"><span data-stu-id="8ec95-112">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="8ec95-113">accountName</span><span class="sxs-lookup"><span data-stu-id="8ec95-113">accountName</span></span>|<span data-ttu-id="8ec95-114">String</span><span class="sxs-lookup"><span data-stu-id="8ec95-114">String</span></span>|<span data-ttu-id="8ec95-115">（没有 Active Directory 域和 DNS 域） 的用户帐户的帐户名 (也称为`mailNickName`)。</span><span class="sxs-lookup"><span data-stu-id="8ec95-115">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="8ec95-116">domainName</span><span class="sxs-lookup"><span data-stu-id="8ec95-116">domainName</span></span>|<span data-ttu-id="8ec95-117">String</span><span class="sxs-lookup"><span data-stu-id="8ec95-117">String</span></span>|<span data-ttu-id="8ec95-118">NetBIOS/Active Directory 域的用户帐户 （即域 \ 帐户格式）。</span><span class="sxs-lookup"><span data-stu-id="8ec95-118">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="8ec95-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="8ec95-119">emailRole</span></span>|<span data-ttu-id="8ec95-120">emailRole</span><span class="sxs-lookup"><span data-stu-id="8ec95-120">emailRole</span></span>|<span data-ttu-id="8ec95-121">电子邮件相关的通知的用户帐户的电子邮件角色。</span><span class="sxs-lookup"><span data-stu-id="8ec95-121">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="8ec95-122">可取值为：`unknown`、`sender`、`recipient`。</span><span class="sxs-lookup"><span data-stu-id="8ec95-122">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="8ec95-123">isVpn</span><span class="sxs-lookup"><span data-stu-id="8ec95-123">isVpn</span></span>|<span data-ttu-id="8ec95-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ec95-124">Boolean</span></span>|<span data-ttu-id="8ec95-125">指示用户是否可以通过 VPN 登录。</span><span class="sxs-lookup"><span data-stu-id="8ec95-125">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="8ec95-126">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="8ec95-126">logonDateTime</span></span>|<span data-ttu-id="8ec95-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ec95-127">DateTimeOffset</span></span>|<span data-ttu-id="8ec95-128">在登录所发生的时间。</span><span class="sxs-lookup"><span data-stu-id="8ec95-128">Time at which the sign-in occurred.</span></span> <span data-ttu-id="8ec95-129">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="8ec95-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8ec95-130">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="8ec95-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="8ec95-131">logonId</span><span class="sxs-lookup"><span data-stu-id="8ec95-131">logonId</span></span>|<span data-ttu-id="8ec95-132">String</span><span class="sxs-lookup"><span data-stu-id="8ec95-132">String</span></span>|<span data-ttu-id="8ec95-133">用户登录 id。</span><span class="sxs-lookup"><span data-stu-id="8ec95-133">User sign-in ID.</span></span>|
|<span data-ttu-id="8ec95-134">logonIp</span><span class="sxs-lookup"><span data-stu-id="8ec95-134">logonIp</span></span>|<span data-ttu-id="8ec95-135">String</span><span class="sxs-lookup"><span data-stu-id="8ec95-135">String</span></span>|<span data-ttu-id="8ec95-136">登录请求源自的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="8ec95-136">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="8ec95-137">logonLocation</span><span class="sxs-lookup"><span data-stu-id="8ec95-137">logonLocation</span></span>|<span data-ttu-id="8ec95-138">String</span><span class="sxs-lookup"><span data-stu-id="8ec95-138">String</span></span>|<span data-ttu-id="8ec95-139">此用户相关联的用户登录事件 （由 IP 地址映射） 位置。</span><span class="sxs-lookup"><span data-stu-id="8ec95-139">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="8ec95-140">logonType</span><span class="sxs-lookup"><span data-stu-id="8ec95-140">logonType</span></span>|<span data-ttu-id="8ec95-141">logonType</span><span class="sxs-lookup"><span data-stu-id="8ec95-141">logonType</span></span>|<span data-ttu-id="8ec95-142">用户登录的方法。</span><span class="sxs-lookup"><span data-stu-id="8ec95-142">Method of user sign in.</span></span> <span data-ttu-id="8ec95-143">可取值为：`unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。</span><span class="sxs-lookup"><span data-stu-id="8ec95-143">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="8ec95-144">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="8ec95-144">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="8ec95-145">String</span><span class="sxs-lookup"><span data-stu-id="8ec95-145">String</span></span>|<span data-ttu-id="8ec95-146">Active Directory （本地） 安全标识符 (SID) 的用户。</span><span class="sxs-lookup"><span data-stu-id="8ec95-146">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="8ec95-147">riskScore</span><span class="sxs-lookup"><span data-stu-id="8ec95-147">riskScore</span></span>|<span data-ttu-id="8ec95-148">String</span><span class="sxs-lookup"><span data-stu-id="8ec95-148">String</span></span>|<span data-ttu-id="8ec95-149">带有提供程序生成/计算风险的用户帐户的分数。</span><span class="sxs-lookup"><span data-stu-id="8ec95-149">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="8ec95-150">建议值的范围为 0-1，这相当于百分比。</span><span class="sxs-lookup"><span data-stu-id="8ec95-150">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="8ec95-151">userAccountType</span><span class="sxs-lookup"><span data-stu-id="8ec95-151">userAccountType</span></span>|<span data-ttu-id="8ec95-152">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="8ec95-152">userAccountSecurityType</span></span>|<span data-ttu-id="8ec95-153">用户帐户类型 （组成员身份），每 Windows 定义。</span><span class="sxs-lookup"><span data-stu-id="8ec95-153">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="8ec95-154">可取值为：`unknown`、`standard`、`power`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="8ec95-154">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="8ec95-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8ec95-155">userPrincipalName</span></span>|<span data-ttu-id="8ec95-156">字符串</span><span class="sxs-lookup"><span data-stu-id="8ec95-156">String</span></span>|<span data-ttu-id="8ec95-157">用户登录名-internet 格式: （用户帐户名） @ （用户帐户 DNS 域名）。</span><span class="sxs-lookup"><span data-stu-id="8ec95-157">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ec95-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8ec95-158">JSON representation</span></span>

<span data-ttu-id="8ec95-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ec95-159">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "userSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/usersecuritystate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
