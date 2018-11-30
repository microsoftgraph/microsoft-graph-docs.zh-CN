---
title: userSecurityState 资源类型
description: 包含状态信息的用户帐户。
ms.openlocfilehash: dbb4b6600cc11a75c84f2f0b233535d012309f88
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010156"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="b507b-103">userSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="b507b-103">userSecurityState resource type</span></span>

<span data-ttu-id="b507b-104">包含状态信息的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="b507b-104">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="b507b-105">属性</span><span class="sxs-lookup"><span data-stu-id="b507b-105">Properties</span></span>

| <span data-ttu-id="b507b-106">属性</span><span class="sxs-lookup"><span data-stu-id="b507b-106">Property</span></span>   | <span data-ttu-id="b507b-107">类型</span><span class="sxs-lookup"><span data-stu-id="b507b-107">Type</span></span> |<span data-ttu-id="b507b-108">说明</span><span class="sxs-lookup"><span data-stu-id="b507b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b507b-109">aadUserId</span><span class="sxs-lookup"><span data-stu-id="b507b-109">aadUserId</span></span>|<span data-ttu-id="b507b-110">字符串</span><span class="sxs-lookup"><span data-stu-id="b507b-110">String</span></span>|<span data-ttu-id="b507b-111">AAD 用户对象标识符 (GUID)-表示物理/多 account 用户实体。</span><span class="sxs-lookup"><span data-stu-id="b507b-111">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="b507b-112">accountName</span><span class="sxs-lookup"><span data-stu-id="b507b-112">accountName</span></span>|<span data-ttu-id="b507b-113">字符串</span><span class="sxs-lookup"><span data-stu-id="b507b-113">String</span></span>|<span data-ttu-id="b507b-114">（没有 Active Directory 域和 DNS 域） 的用户帐户的帐户名 (也称为`mailNickName`)。</span><span class="sxs-lookup"><span data-stu-id="b507b-114">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="b507b-115">domainName</span><span class="sxs-lookup"><span data-stu-id="b507b-115">domainName</span></span>|<span data-ttu-id="b507b-116">String</span><span class="sxs-lookup"><span data-stu-id="b507b-116">String</span></span>|<span data-ttu-id="b507b-117">NetBIOS/Active Directory 域的用户帐户 （即域 \ 帐户格式）。</span><span class="sxs-lookup"><span data-stu-id="b507b-117">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="b507b-118">emailRole</span><span class="sxs-lookup"><span data-stu-id="b507b-118">emailRole</span></span>|<span data-ttu-id="b507b-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="b507b-119">emailRole</span></span>|<span data-ttu-id="b507b-120">电子邮件相关的通知的用户帐户的电子邮件角色。</span><span class="sxs-lookup"><span data-stu-id="b507b-120">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="b507b-121">可取值为：`unknown`、`sender`、`recipient`。</span><span class="sxs-lookup"><span data-stu-id="b507b-121">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="b507b-122">isVpn</span><span class="sxs-lookup"><span data-stu-id="b507b-122">isVpn</span></span>|<span data-ttu-id="b507b-123">布尔</span><span class="sxs-lookup"><span data-stu-id="b507b-123">Boolean</span></span>|<span data-ttu-id="b507b-124">指示用户是否可以通过 VPN 登录。</span><span class="sxs-lookup"><span data-stu-id="b507b-124">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="b507b-125">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="b507b-125">logonDateTime</span></span>|<span data-ttu-id="b507b-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b507b-126">DateTimeOffset</span></span>|<span data-ttu-id="b507b-127">在登录所发生的时间。</span><span class="sxs-lookup"><span data-stu-id="b507b-127">Time at which the sign-in occurred.</span></span> <span data-ttu-id="b507b-128">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="b507b-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b507b-129">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="b507b-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="b507b-130">logonId</span><span class="sxs-lookup"><span data-stu-id="b507b-130">logonId</span></span>|<span data-ttu-id="b507b-131">字符串</span><span class="sxs-lookup"><span data-stu-id="b507b-131">String</span></span>|<span data-ttu-id="b507b-132">用户登录 id。</span><span class="sxs-lookup"><span data-stu-id="b507b-132">User sign-in ID.</span></span>|
|<span data-ttu-id="b507b-133">logonIp</span><span class="sxs-lookup"><span data-stu-id="b507b-133">logonIp</span></span>|<span data-ttu-id="b507b-134">字符串</span><span class="sxs-lookup"><span data-stu-id="b507b-134">String</span></span>|<span data-ttu-id="b507b-135">登录请求源自的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="b507b-135">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="b507b-136">logonLocation</span><span class="sxs-lookup"><span data-stu-id="b507b-136">logonLocation</span></span>|<span data-ttu-id="b507b-137">字符串</span><span class="sxs-lookup"><span data-stu-id="b507b-137">String</span></span>|<span data-ttu-id="b507b-138">此用户相关联的用户登录事件 （由 IP 地址映射） 位置。</span><span class="sxs-lookup"><span data-stu-id="b507b-138">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="b507b-139">logonType</span><span class="sxs-lookup"><span data-stu-id="b507b-139">logonType</span></span>|<span data-ttu-id="b507b-140">logonType</span><span class="sxs-lookup"><span data-stu-id="b507b-140">logonType</span></span>|<span data-ttu-id="b507b-141">用户登录的方法。</span><span class="sxs-lookup"><span data-stu-id="b507b-141">Method of user sign in.</span></span> <span data-ttu-id="b507b-142">可取值为：`unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。</span><span class="sxs-lookup"><span data-stu-id="b507b-142">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="b507b-143">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="b507b-143">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="b507b-144">字符串</span><span class="sxs-lookup"><span data-stu-id="b507b-144">String</span></span>|<span data-ttu-id="b507b-145">Active Directory （本地） 安全标识符 (SID) 的用户。</span><span class="sxs-lookup"><span data-stu-id="b507b-145">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="b507b-146">riskScore</span><span class="sxs-lookup"><span data-stu-id="b507b-146">riskScore</span></span>|<span data-ttu-id="b507b-147">字符串</span><span class="sxs-lookup"><span data-stu-id="b507b-147">String</span></span>|<span data-ttu-id="b507b-148">带有提供程序生成/计算风险的用户帐户的分数。</span><span class="sxs-lookup"><span data-stu-id="b507b-148">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="b507b-149">建议值的范围为 0-1，这相当于百分比。</span><span class="sxs-lookup"><span data-stu-id="b507b-149">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="b507b-150">userAccountType</span><span class="sxs-lookup"><span data-stu-id="b507b-150">userAccountType</span></span>|<span data-ttu-id="b507b-151">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="b507b-151">userAccountSecurityType</span></span>|<span data-ttu-id="b507b-152">用户帐户类型 （组成员身份），每 Windows 定义。</span><span class="sxs-lookup"><span data-stu-id="b507b-152">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="b507b-153">可取值为：`unknown`、`standard`、`power`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="b507b-153">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="b507b-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b507b-154">userPrincipalName</span></span>|<span data-ttu-id="b507b-155">字符串</span><span class="sxs-lookup"><span data-stu-id="b507b-155">String</span></span>|<span data-ttu-id="b507b-156">用户登录名-internet 格式: （用户帐户名） @ （用户帐户 DNS 域名）。</span><span class="sxs-lookup"><span data-stu-id="b507b-156">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b507b-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b507b-157">JSON representation</span></span>

<span data-ttu-id="b507b-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b507b-158">The following is a JSON representation of the resource.</span></span>

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
