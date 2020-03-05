---
title: Logonip 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 67e5c7d2feb76346d754f582e34b5afe39af3d32
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519510"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="b4b83-104">Logonip 资源类型</span><span class="sxs-lookup"><span data-stu-id="b4b83-104">userSecurityState resource type</span></span>

<span data-ttu-id="b4b83-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b4b83-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4b83-106">包含有关用户帐户的状态信息。</span><span class="sxs-lookup"><span data-stu-id="b4b83-106">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="b4b83-107">属性</span><span class="sxs-lookup"><span data-stu-id="b4b83-107">Properties</span></span>

| <span data-ttu-id="b4b83-108">属性</span><span class="sxs-lookup"><span data-stu-id="b4b83-108">Property</span></span>   | <span data-ttu-id="b4b83-109">类型</span><span class="sxs-lookup"><span data-stu-id="b4b83-109">Type</span></span> |<span data-ttu-id="b4b83-110">说明</span><span class="sxs-lookup"><span data-stu-id="b4b83-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4b83-111">aadUserId</span><span class="sxs-lookup"><span data-stu-id="b4b83-111">aadUserId</span></span>|<span data-ttu-id="b4b83-112">String</span><span class="sxs-lookup"><span data-stu-id="b4b83-112">String</span></span>|<span data-ttu-id="b4b83-113">AAD 用户对象标识符（GUID）-表示物理/多帐户用户实体。</span><span class="sxs-lookup"><span data-stu-id="b4b83-113">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="b4b83-114">帐户</span><span class="sxs-lookup"><span data-stu-id="b4b83-114">accountName</span></span>|<span data-ttu-id="b4b83-115">String</span><span class="sxs-lookup"><span data-stu-id="b4b83-115">String</span></span>|<span data-ttu-id="b4b83-116">用户帐户的帐户名（不包含 Active Directory 域或 DNS 域）-（也`mailNickName`称为）。</span><span class="sxs-lookup"><span data-stu-id="b4b83-116">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="b4b83-117">domainName</span><span class="sxs-lookup"><span data-stu-id="b4b83-117">domainName</span></span>|<span data-ttu-id="b4b83-118">String</span><span class="sxs-lookup"><span data-stu-id="b4b83-118">String</span></span>|<span data-ttu-id="b4b83-119">用户帐户的 NetBIOS/Active Directory 域（即，域 \ 帐户格式）。</span><span class="sxs-lookup"><span data-stu-id="b4b83-119">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="b4b83-120">emailRole</span><span class="sxs-lookup"><span data-stu-id="b4b83-120">emailRole</span></span>|<span data-ttu-id="b4b83-121">emailRole</span><span class="sxs-lookup"><span data-stu-id="b4b83-121">emailRole</span></span>|<span data-ttu-id="b4b83-122">对于与电子邮件相关的警报-用户帐户的电子邮件 "role"。</span><span class="sxs-lookup"><span data-stu-id="b4b83-122">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="b4b83-123">可取值为：`unknown`、`sender`、`recipient`。</span><span class="sxs-lookup"><span data-stu-id="b4b83-123">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="b4b83-124">isVpn</span><span class="sxs-lookup"><span data-stu-id="b4b83-124">isVpn</span></span>|<span data-ttu-id="b4b83-125">布尔</span><span class="sxs-lookup"><span data-stu-id="b4b83-125">Boolean</span></span>|<span data-ttu-id="b4b83-126">指示用户是否通过 VPN 登录。</span><span class="sxs-lookup"><span data-stu-id="b4b83-126">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="b4b83-127">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="b4b83-127">logonDateTime</span></span>|<span data-ttu-id="b4b83-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4b83-128">DateTimeOffset</span></span>|<span data-ttu-id="b4b83-129">登录发生的时间。</span><span class="sxs-lookup"><span data-stu-id="b4b83-129">Time at which the sign-in occurred.</span></span> <span data-ttu-id="b4b83-130">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="b4b83-130">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b4b83-131">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="b4b83-131">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="b4b83-132">logonId</span><span class="sxs-lookup"><span data-stu-id="b4b83-132">logonId</span></span>|<span data-ttu-id="b4b83-133">String</span><span class="sxs-lookup"><span data-stu-id="b4b83-133">String</span></span>|<span data-ttu-id="b4b83-134">用户登录 ID。</span><span class="sxs-lookup"><span data-stu-id="b4b83-134">User sign-in ID.</span></span>|
|<span data-ttu-id="b4b83-135">Usersecuritystate</span><span class="sxs-lookup"><span data-stu-id="b4b83-135">logonIp</span></span>|<span data-ttu-id="b4b83-136">String</span><span class="sxs-lookup"><span data-stu-id="b4b83-136">String</span></span>|<span data-ttu-id="b4b83-137">发出登录请求的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="b4b83-137">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="b4b83-138">logonLocation</span><span class="sxs-lookup"><span data-stu-id="b4b83-138">logonLocation</span></span>|<span data-ttu-id="b4b83-139">String</span><span class="sxs-lookup"><span data-stu-id="b4b83-139">String</span></span>|<span data-ttu-id="b4b83-140">与用户登录事件关联的此用户的位置（按 IP 地址映射）。</span><span class="sxs-lookup"><span data-stu-id="b4b83-140">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="b4b83-141">logonType</span><span class="sxs-lookup"><span data-stu-id="b4b83-141">logonType</span></span>|<span data-ttu-id="b4b83-142">logonType</span><span class="sxs-lookup"><span data-stu-id="b4b83-142">logonType</span></span>|<span data-ttu-id="b4b83-143">用户登录的方法。</span><span class="sxs-lookup"><span data-stu-id="b4b83-143">Method of user sign in.</span></span> <span data-ttu-id="b4b83-144">可取值为：`unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。</span><span class="sxs-lookup"><span data-stu-id="b4b83-144">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="b4b83-145">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="b4b83-145">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="b4b83-146">字符串</span><span class="sxs-lookup"><span data-stu-id="b4b83-146">String</span></span>|<span data-ttu-id="b4b83-147">用户的 Active Directory （本地）安全标识符（SID）。</span><span class="sxs-lookup"><span data-stu-id="b4b83-147">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="b4b83-148">riskScore</span><span class="sxs-lookup"><span data-stu-id="b4b83-148">riskScore</span></span>|<span data-ttu-id="b4b83-149">String</span><span class="sxs-lookup"><span data-stu-id="b4b83-149">String</span></span>|<span data-ttu-id="b4b83-150">提供程序生成/计算的风险分数的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="b4b83-150">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="b4b83-151">建议的值范围为0-1，这相当于一个百分比。</span><span class="sxs-lookup"><span data-stu-id="b4b83-151">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="b4b83-152">userAccountType</span><span class="sxs-lookup"><span data-stu-id="b4b83-152">userAccountType</span></span>|<span data-ttu-id="b4b83-153">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="b4b83-153">userAccountSecurityType</span></span>|<span data-ttu-id="b4b83-154">每个 Windows 定义的用户帐户类型（组成员身份）。</span><span class="sxs-lookup"><span data-stu-id="b4b83-154">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="b4b83-155">可取值为：`unknown`、`standard`、`power`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="b4b83-155">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="b4b83-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b4b83-156">userPrincipalName</span></span>|<span data-ttu-id="b4b83-157">String</span><span class="sxs-lookup"><span data-stu-id="b4b83-157">String</span></span>|<span data-ttu-id="b4b83-158">用户登录名-internet 格式：（用户帐户名称） @ （用户帐户 DNS 域名）。</span><span class="sxs-lookup"><span data-stu-id="b4b83-158">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b4b83-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b4b83-159">JSON representation</span></span>

<span data-ttu-id="b4b83-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4b83-160">The following is a JSON representation of the resource.</span></span>

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
