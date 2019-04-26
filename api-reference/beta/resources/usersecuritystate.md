---
title: logonip 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。"
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7ca02b6582898e8a0184c6c37115c9ac96b386ff
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345065"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="956d9-104">logonip 资源类型</span><span class="sxs-lookup"><span data-stu-id="956d9-104">userSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="956d9-105">包含有关用户帐户的状态信息。</span><span class="sxs-lookup"><span data-stu-id="956d9-105">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="956d9-106">属性</span><span class="sxs-lookup"><span data-stu-id="956d9-106">Properties</span></span>

| <span data-ttu-id="956d9-107">属性</span><span class="sxs-lookup"><span data-stu-id="956d9-107">Property</span></span>   | <span data-ttu-id="956d9-108">类型</span><span class="sxs-lookup"><span data-stu-id="956d9-108">Type</span></span> |<span data-ttu-id="956d9-109">说明</span><span class="sxs-lookup"><span data-stu-id="956d9-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="956d9-110">aadUserId</span><span class="sxs-lookup"><span data-stu-id="956d9-110">aadUserId</span></span>|<span data-ttu-id="956d9-111">String</span><span class="sxs-lookup"><span data-stu-id="956d9-111">String</span></span>|<span data-ttu-id="956d9-112">AAD 用户对象标识符 (GUID)-表示物理/多帐户用户实体。</span><span class="sxs-lookup"><span data-stu-id="956d9-112">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="956d9-113">帐户</span><span class="sxs-lookup"><span data-stu-id="956d9-113">accountName</span></span>|<span data-ttu-id="956d9-114">String</span><span class="sxs-lookup"><span data-stu-id="956d9-114">String</span></span>|<span data-ttu-id="956d9-115">用户帐户的帐户名 (不包含 Active Directory 域或 DNS 域)-(也`mailNickName`称为)。</span><span class="sxs-lookup"><span data-stu-id="956d9-115">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="956d9-116">domainName</span><span class="sxs-lookup"><span data-stu-id="956d9-116">domainName</span></span>|<span data-ttu-id="956d9-117">String</span><span class="sxs-lookup"><span data-stu-id="956d9-117">String</span></span>|<span data-ttu-id="956d9-118">用户帐户的 NetBIOS/Active Directory 域 (即, 域 \ 帐户格式)。</span><span class="sxs-lookup"><span data-stu-id="956d9-118">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="956d9-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="956d9-119">emailRole</span></span>|<span data-ttu-id="956d9-120">emailRole</span><span class="sxs-lookup"><span data-stu-id="956d9-120">emailRole</span></span>|<span data-ttu-id="956d9-121">对于与电子邮件相关的警报-用户帐户的电子邮件 "role"。</span><span class="sxs-lookup"><span data-stu-id="956d9-121">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="956d9-122">可取值为：`unknown`、`sender`、`recipient`。</span><span class="sxs-lookup"><span data-stu-id="956d9-122">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="956d9-123">isVpn</span><span class="sxs-lookup"><span data-stu-id="956d9-123">isVpn</span></span>|<span data-ttu-id="956d9-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="956d9-124">Boolean</span></span>|<span data-ttu-id="956d9-125">指示用户是否通过 VPN 登录。</span><span class="sxs-lookup"><span data-stu-id="956d9-125">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="956d9-126">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="956d9-126">logonDateTime</span></span>|<span data-ttu-id="956d9-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="956d9-127">DateTimeOffset</span></span>|<span data-ttu-id="956d9-128">登录发生的时间。</span><span class="sxs-lookup"><span data-stu-id="956d9-128">Time at which the sign-in occurred.</span></span> <span data-ttu-id="956d9-129">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="956d9-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="956d9-130">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="956d9-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="956d9-131">logonId</span><span class="sxs-lookup"><span data-stu-id="956d9-131">logonId</span></span>|<span data-ttu-id="956d9-132">String</span><span class="sxs-lookup"><span data-stu-id="956d9-132">String</span></span>|<span data-ttu-id="956d9-133">用户登录 ID。</span><span class="sxs-lookup"><span data-stu-id="956d9-133">User sign-in ID.</span></span>|
|<span data-ttu-id="956d9-134">usersecuritystate</span><span class="sxs-lookup"><span data-stu-id="956d9-134">logonIp</span></span>|<span data-ttu-id="956d9-135">String</span><span class="sxs-lookup"><span data-stu-id="956d9-135">String</span></span>|<span data-ttu-id="956d9-136">发出登录请求的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="956d9-136">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="956d9-137">logonLocation</span><span class="sxs-lookup"><span data-stu-id="956d9-137">logonLocation</span></span>|<span data-ttu-id="956d9-138">String</span><span class="sxs-lookup"><span data-stu-id="956d9-138">String</span></span>|<span data-ttu-id="956d9-139">与用户登录事件关联的此用户的位置 (按 IP 地址映射)。</span><span class="sxs-lookup"><span data-stu-id="956d9-139">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="956d9-140">logonType</span><span class="sxs-lookup"><span data-stu-id="956d9-140">logonType</span></span>|<span data-ttu-id="956d9-141">logonType</span><span class="sxs-lookup"><span data-stu-id="956d9-141">logonType</span></span>|<span data-ttu-id="956d9-142">用户登录的方法。</span><span class="sxs-lookup"><span data-stu-id="956d9-142">Method of user sign in.</span></span> <span data-ttu-id="956d9-143">可取值为：`unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。</span><span class="sxs-lookup"><span data-stu-id="956d9-143">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="956d9-144">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="956d9-144">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="956d9-145">字符串</span><span class="sxs-lookup"><span data-stu-id="956d9-145">String</span></span>|<span data-ttu-id="956d9-146">用户的 Active Directory (本地) 安全标识符 (SID)。</span><span class="sxs-lookup"><span data-stu-id="956d9-146">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="956d9-147">riskScore</span><span class="sxs-lookup"><span data-stu-id="956d9-147">riskScore</span></span>|<span data-ttu-id="956d9-148">String</span><span class="sxs-lookup"><span data-stu-id="956d9-148">String</span></span>|<span data-ttu-id="956d9-149">提供程序生成/计算的风险分数的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="956d9-149">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="956d9-150">建议的值范围为 0-1, 这相当于一个百分比。</span><span class="sxs-lookup"><span data-stu-id="956d9-150">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="956d9-151">userAccountType</span><span class="sxs-lookup"><span data-stu-id="956d9-151">userAccountType</span></span>|<span data-ttu-id="956d9-152">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="956d9-152">userAccountSecurityType</span></span>|<span data-ttu-id="956d9-153">每个 Windows 定义的用户帐户类型 (组成员身份)。</span><span class="sxs-lookup"><span data-stu-id="956d9-153">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="956d9-154">可取值为：`unknown`、`standard`、`power`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="956d9-154">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="956d9-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="956d9-155">userPrincipalName</span></span>|<span data-ttu-id="956d9-156">String</span><span class="sxs-lookup"><span data-stu-id="956d9-156">String</span></span>|<span data-ttu-id="956d9-157">用户登录名-internet 格式: (用户帐户名称) @ (用户帐户 DNS 域名)。</span><span class="sxs-lookup"><span data-stu-id="956d9-157">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="956d9-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="956d9-158">JSON representation</span></span>

<span data-ttu-id="956d9-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="956d9-159">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
