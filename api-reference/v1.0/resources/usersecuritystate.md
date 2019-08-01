---
title: Logonip 资源类型
description: 包含有关用户帐户的状态信息。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9f5a856a9ec04eaf9a04b82e2ed7697a6735ad88
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033472"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="48c2d-103">Logonip 资源类型</span><span class="sxs-lookup"><span data-stu-id="48c2d-103">userSecurityState resource type</span></span>

<span data-ttu-id="48c2d-104">包含有关用户帐户的状态信息。</span><span class="sxs-lookup"><span data-stu-id="48c2d-104">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="48c2d-105">属性</span><span class="sxs-lookup"><span data-stu-id="48c2d-105">Properties</span></span>

| <span data-ttu-id="48c2d-106">属性</span><span class="sxs-lookup"><span data-stu-id="48c2d-106">Property</span></span>   | <span data-ttu-id="48c2d-107">类型</span><span class="sxs-lookup"><span data-stu-id="48c2d-107">Type</span></span> |<span data-ttu-id="48c2d-108">说明</span><span class="sxs-lookup"><span data-stu-id="48c2d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48c2d-109">aadUserId</span><span class="sxs-lookup"><span data-stu-id="48c2d-109">aadUserId</span></span>|<span data-ttu-id="48c2d-110">String</span><span class="sxs-lookup"><span data-stu-id="48c2d-110">String</span></span>|<span data-ttu-id="48c2d-111">AAD 用户对象标识符 (GUID)-表示物理/多帐户用户实体。</span><span class="sxs-lookup"><span data-stu-id="48c2d-111">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="48c2d-112">帐户</span><span class="sxs-lookup"><span data-stu-id="48c2d-112">accountName</span></span>|<span data-ttu-id="48c2d-113">String</span><span class="sxs-lookup"><span data-stu-id="48c2d-113">String</span></span>|<span data-ttu-id="48c2d-114">用户帐户的帐户名 (不包含 Active Directory 域或 DNS 域)-(也`mailNickName`称为)。</span><span class="sxs-lookup"><span data-stu-id="48c2d-114">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="48c2d-115">domainName</span><span class="sxs-lookup"><span data-stu-id="48c2d-115">domainName</span></span>|<span data-ttu-id="48c2d-116">String</span><span class="sxs-lookup"><span data-stu-id="48c2d-116">String</span></span>|<span data-ttu-id="48c2d-117">用户帐户的 NetBIOS/Active Directory 域 (即, 域 \ 帐户格式)。</span><span class="sxs-lookup"><span data-stu-id="48c2d-117">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="48c2d-118">emailRole</span><span class="sxs-lookup"><span data-stu-id="48c2d-118">emailRole</span></span>|<span data-ttu-id="48c2d-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="48c2d-119">emailRole</span></span>|<span data-ttu-id="48c2d-120">对于与电子邮件相关的警报-用户帐户的电子邮件 "role"。</span><span class="sxs-lookup"><span data-stu-id="48c2d-120">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="48c2d-121">可取值为：`unknown`、`sender`、`recipient`。</span><span class="sxs-lookup"><span data-stu-id="48c2d-121">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="48c2d-122">isVpn</span><span class="sxs-lookup"><span data-stu-id="48c2d-122">isVpn</span></span>|<span data-ttu-id="48c2d-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="48c2d-123">Boolean</span></span>|<span data-ttu-id="48c2d-124">指示用户是否通过 VPN 登录。</span><span class="sxs-lookup"><span data-stu-id="48c2d-124">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="48c2d-125">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="48c2d-125">logonDateTime</span></span>|<span data-ttu-id="48c2d-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48c2d-126">DateTimeOffset</span></span>|<span data-ttu-id="48c2d-127">登录发生的时间。</span><span class="sxs-lookup"><span data-stu-id="48c2d-127">Time at which the sign-in occurred.</span></span> <span data-ttu-id="48c2d-128">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="48c2d-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="48c2d-129">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="48c2d-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="48c2d-130">logonId</span><span class="sxs-lookup"><span data-stu-id="48c2d-130">logonId</span></span>|<span data-ttu-id="48c2d-131">String</span><span class="sxs-lookup"><span data-stu-id="48c2d-131">String</span></span>|<span data-ttu-id="48c2d-132">用户登录 ID。</span><span class="sxs-lookup"><span data-stu-id="48c2d-132">User sign-in ID.</span></span>|
|<span data-ttu-id="48c2d-133">Usersecuritystate</span><span class="sxs-lookup"><span data-stu-id="48c2d-133">logonIp</span></span>|<span data-ttu-id="48c2d-134">String</span><span class="sxs-lookup"><span data-stu-id="48c2d-134">String</span></span>|<span data-ttu-id="48c2d-135">发出登录请求的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="48c2d-135">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="48c2d-136">logonLocation</span><span class="sxs-lookup"><span data-stu-id="48c2d-136">logonLocation</span></span>|<span data-ttu-id="48c2d-137">String</span><span class="sxs-lookup"><span data-stu-id="48c2d-137">String</span></span>|<span data-ttu-id="48c2d-138">与用户登录事件关联的此用户的位置 (按 IP 地址映射)。</span><span class="sxs-lookup"><span data-stu-id="48c2d-138">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="48c2d-139">logonType</span><span class="sxs-lookup"><span data-stu-id="48c2d-139">logonType</span></span>|<span data-ttu-id="48c2d-140">logonType</span><span class="sxs-lookup"><span data-stu-id="48c2d-140">logonType</span></span>|<span data-ttu-id="48c2d-141">用户登录的方法。</span><span class="sxs-lookup"><span data-stu-id="48c2d-141">Method of user sign in.</span></span> <span data-ttu-id="48c2d-142">可取值为：`unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。</span><span class="sxs-lookup"><span data-stu-id="48c2d-142">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="48c2d-143">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="48c2d-143">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="48c2d-144">字符串</span><span class="sxs-lookup"><span data-stu-id="48c2d-144">String</span></span>|<span data-ttu-id="48c2d-145">用户的 Active Directory (本地) 安全标识符 (SID)。</span><span class="sxs-lookup"><span data-stu-id="48c2d-145">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="48c2d-146">riskScore</span><span class="sxs-lookup"><span data-stu-id="48c2d-146">riskScore</span></span>|<span data-ttu-id="48c2d-147">String</span><span class="sxs-lookup"><span data-stu-id="48c2d-147">String</span></span>|<span data-ttu-id="48c2d-148">提供程序生成/计算的风险分数的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="48c2d-148">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="48c2d-149">建议的值范围为 0-1, 这相当于一个百分比。</span><span class="sxs-lookup"><span data-stu-id="48c2d-149">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="48c2d-150">userAccountType</span><span class="sxs-lookup"><span data-stu-id="48c2d-150">userAccountType</span></span>|<span data-ttu-id="48c2d-151">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="48c2d-151">userAccountSecurityType</span></span>|<span data-ttu-id="48c2d-152">每个 Windows 定义的用户帐户类型 (组成员身份)。</span><span class="sxs-lookup"><span data-stu-id="48c2d-152">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="48c2d-153">可取值为：`unknown`、`standard`、`power`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="48c2d-153">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="48c2d-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="48c2d-154">userPrincipalName</span></span>|<span data-ttu-id="48c2d-155">String</span><span class="sxs-lookup"><span data-stu-id="48c2d-155">String</span></span>|<span data-ttu-id="48c2d-156">用户登录名-internet 格式: (用户帐户名称) @ (用户帐户 DNS 域名)。</span><span class="sxs-lookup"><span data-stu-id="48c2d-156">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="48c2d-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="48c2d-157">JSON representation</span></span>

<span data-ttu-id="48c2d-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48c2d-158">The following is a JSON representation of the resource.</span></span>

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
