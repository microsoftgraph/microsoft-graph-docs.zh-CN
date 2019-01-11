---
title: userSecurityState 资源类型
description: 包含状态信息的用户帐户。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 9d972ee674fbd1553e2b76a52876bc50274466c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845848"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="8d2ea-103">userSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d2ea-103">userSecurityState resource type</span></span>

<span data-ttu-id="8d2ea-104">包含状态信息的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="8d2ea-104">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="8d2ea-105">属性</span><span class="sxs-lookup"><span data-stu-id="8d2ea-105">Properties</span></span>

| <span data-ttu-id="8d2ea-106">属性</span><span class="sxs-lookup"><span data-stu-id="8d2ea-106">Property</span></span>   | <span data-ttu-id="8d2ea-107">类型</span><span class="sxs-lookup"><span data-stu-id="8d2ea-107">Type</span></span> |<span data-ttu-id="8d2ea-108">Description</span><span class="sxs-lookup"><span data-stu-id="8d2ea-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d2ea-109">aadUserId</span><span class="sxs-lookup"><span data-stu-id="8d2ea-109">aadUserId</span></span>|<span data-ttu-id="8d2ea-110">字符串</span><span class="sxs-lookup"><span data-stu-id="8d2ea-110">String</span></span>|<span data-ttu-id="8d2ea-111">AAD 用户对象标识符 (GUID)-表示物理/多 account 用户实体。</span><span class="sxs-lookup"><span data-stu-id="8d2ea-111">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="8d2ea-112">accountName</span><span class="sxs-lookup"><span data-stu-id="8d2ea-112">accountName</span></span>|<span data-ttu-id="8d2ea-113">字符串</span><span class="sxs-lookup"><span data-stu-id="8d2ea-113">String</span></span>|<span data-ttu-id="8d2ea-114">（没有 Active Directory 域和 DNS 域） 的用户帐户的帐户名 (也称为`mailNickName`)。</span><span class="sxs-lookup"><span data-stu-id="8d2ea-114">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="8d2ea-115">domainName</span><span class="sxs-lookup"><span data-stu-id="8d2ea-115">domainName</span></span>|<span data-ttu-id="8d2ea-116">String</span><span class="sxs-lookup"><span data-stu-id="8d2ea-116">String</span></span>|<span data-ttu-id="8d2ea-117">NetBIOS/Active Directory 域的用户帐户 （即域 \ 帐户格式）。</span><span class="sxs-lookup"><span data-stu-id="8d2ea-117">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="8d2ea-118">emailRole</span><span class="sxs-lookup"><span data-stu-id="8d2ea-118">emailRole</span></span>|<span data-ttu-id="8d2ea-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="8d2ea-119">emailRole</span></span>|<span data-ttu-id="8d2ea-120">电子邮件相关的通知的用户帐户的电子邮件角色。</span><span class="sxs-lookup"><span data-stu-id="8d2ea-120">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="8d2ea-121">可取值为：`unknown`、`sender`、`recipient`。</span><span class="sxs-lookup"><span data-stu-id="8d2ea-121">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="8d2ea-122">isVpn</span><span class="sxs-lookup"><span data-stu-id="8d2ea-122">isVpn</span></span>|<span data-ttu-id="8d2ea-123">布尔</span><span class="sxs-lookup"><span data-stu-id="8d2ea-123">Boolean</span></span>|<span data-ttu-id="8d2ea-124">指示用户是否可以通过 VPN 登录。</span><span class="sxs-lookup"><span data-stu-id="8d2ea-124">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="8d2ea-125">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="8d2ea-125">logonDateTime</span></span>|<span data-ttu-id="8d2ea-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d2ea-126">DateTimeOffset</span></span>|<span data-ttu-id="8d2ea-127">在登录所发生的时间。</span><span class="sxs-lookup"><span data-stu-id="8d2ea-127">Time at which the sign-in occurred.</span></span> <span data-ttu-id="8d2ea-128">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="8d2ea-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8d2ea-129">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="8d2ea-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="8d2ea-130">logonId</span><span class="sxs-lookup"><span data-stu-id="8d2ea-130">logonId</span></span>|<span data-ttu-id="8d2ea-131">字符串</span><span class="sxs-lookup"><span data-stu-id="8d2ea-131">String</span></span>|<span data-ttu-id="8d2ea-132">用户登录 id。</span><span class="sxs-lookup"><span data-stu-id="8d2ea-132">User sign-in ID.</span></span>|
|<span data-ttu-id="8d2ea-133">logonIp</span><span class="sxs-lookup"><span data-stu-id="8d2ea-133">logonIp</span></span>|<span data-ttu-id="8d2ea-134">字符串</span><span class="sxs-lookup"><span data-stu-id="8d2ea-134">String</span></span>|<span data-ttu-id="8d2ea-135">登录请求源自的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="8d2ea-135">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="8d2ea-136">logonLocation</span><span class="sxs-lookup"><span data-stu-id="8d2ea-136">logonLocation</span></span>|<span data-ttu-id="8d2ea-137">字符串</span><span class="sxs-lookup"><span data-stu-id="8d2ea-137">String</span></span>|<span data-ttu-id="8d2ea-138">此用户相关联的用户登录事件 （由 IP 地址映射） 位置。</span><span class="sxs-lookup"><span data-stu-id="8d2ea-138">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="8d2ea-139">logonType</span><span class="sxs-lookup"><span data-stu-id="8d2ea-139">logonType</span></span>|<span data-ttu-id="8d2ea-140">logonType</span><span class="sxs-lookup"><span data-stu-id="8d2ea-140">logonType</span></span>|<span data-ttu-id="8d2ea-141">用户登录的方法。</span><span class="sxs-lookup"><span data-stu-id="8d2ea-141">Method of user sign in.</span></span> <span data-ttu-id="8d2ea-142">可取值为：`unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。</span><span class="sxs-lookup"><span data-stu-id="8d2ea-142">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="8d2ea-143">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="8d2ea-143">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="8d2ea-144">字符串</span><span class="sxs-lookup"><span data-stu-id="8d2ea-144">String</span></span>|<span data-ttu-id="8d2ea-145">Active Directory （本地） 安全标识符 (SID) 的用户。</span><span class="sxs-lookup"><span data-stu-id="8d2ea-145">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="8d2ea-146">riskScore</span><span class="sxs-lookup"><span data-stu-id="8d2ea-146">riskScore</span></span>|<span data-ttu-id="8d2ea-147">字符串</span><span class="sxs-lookup"><span data-stu-id="8d2ea-147">String</span></span>|<span data-ttu-id="8d2ea-148">带有提供程序生成/计算风险的用户帐户的分数。</span><span class="sxs-lookup"><span data-stu-id="8d2ea-148">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="8d2ea-149">建议值的范围为 0-1，这相当于百分比。</span><span class="sxs-lookup"><span data-stu-id="8d2ea-149">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="8d2ea-150">userAccountType</span><span class="sxs-lookup"><span data-stu-id="8d2ea-150">userAccountType</span></span>|<span data-ttu-id="8d2ea-151">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="8d2ea-151">userAccountSecurityType</span></span>|<span data-ttu-id="8d2ea-152">用户帐户类型 （组成员身份），每 Windows 定义。</span><span class="sxs-lookup"><span data-stu-id="8d2ea-152">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="8d2ea-153">可取值为：`unknown`、`standard`、`power`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="8d2ea-153">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="8d2ea-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8d2ea-154">userPrincipalName</span></span>|<span data-ttu-id="8d2ea-155">字符串</span><span class="sxs-lookup"><span data-stu-id="8d2ea-155">String</span></span>|<span data-ttu-id="8d2ea-156">用户登录名-internet 格式: （用户帐户名） @ （用户帐户 DNS 域名）。</span><span class="sxs-lookup"><span data-stu-id="8d2ea-156">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d2ea-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d2ea-157">JSON representation</span></span>

<span data-ttu-id="8d2ea-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d2ea-158">The following is a JSON representation of the resource.</span></span>

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
