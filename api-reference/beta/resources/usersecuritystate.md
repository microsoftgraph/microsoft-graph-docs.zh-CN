---
title: userSecurityState 资源类型
description: 包含有关用户帐户的有状态信息。
localization_priority: Normal
author: jpettere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: edd3f3eeb4e8efffde9abd4a8fb53a8a5ddb9ea3
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722256"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="05e11-103">userSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="05e11-103">userSecurityState resource type</span></span>

<span data-ttu-id="05e11-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05e11-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05e11-105">包含有关用户帐户的有状态信息。</span><span class="sxs-lookup"><span data-stu-id="05e11-105">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="05e11-106">属性</span><span class="sxs-lookup"><span data-stu-id="05e11-106">Properties</span></span>

| <span data-ttu-id="05e11-107">属性</span><span class="sxs-lookup"><span data-stu-id="05e11-107">Property</span></span>   | <span data-ttu-id="05e11-108">类型</span><span class="sxs-lookup"><span data-stu-id="05e11-108">Type</span></span> |<span data-ttu-id="05e11-109">说明</span><span class="sxs-lookup"><span data-stu-id="05e11-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05e11-110">aadUserId</span><span class="sxs-lookup"><span data-stu-id="05e11-110">aadUserId</span></span>|<span data-ttu-id="05e11-111">String</span><span class="sxs-lookup"><span data-stu-id="05e11-111">String</span></span>|<span data-ttu-id="05e11-112">AAD 用户对象标识符 (GUID) - 表示物理/多帐户用户实体。</span><span class="sxs-lookup"><span data-stu-id="05e11-112">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="05e11-113">accountName</span><span class="sxs-lookup"><span data-stu-id="05e11-113">accountName</span></span>|<span data-ttu-id="05e11-114">String</span><span class="sxs-lookup"><span data-stu-id="05e11-114">String</span></span>|<span data-ttu-id="05e11-115">没有 Active Directory 域或 DNS 域 (用户帐户的帐户) - (也称为 `mailNickName`) 。</span><span class="sxs-lookup"><span data-stu-id="05e11-115">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="05e11-116">domainName</span><span class="sxs-lookup"><span data-stu-id="05e11-116">domainName</span></span>|<span data-ttu-id="05e11-117">String</span><span class="sxs-lookup"><span data-stu-id="05e11-117">String</span></span>|<span data-ttu-id="05e11-118">用户帐户的 NetBIOS/Active Directory (，即域\帐户) 。</span><span class="sxs-lookup"><span data-stu-id="05e11-118">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="05e11-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="05e11-119">emailRole</span></span>|<span data-ttu-id="05e11-120">emailRole</span><span class="sxs-lookup"><span data-stu-id="05e11-120">emailRole</span></span>|<span data-ttu-id="05e11-121">对于电子邮件相关警报 - 用户帐户的电子邮件"角色"。</span><span class="sxs-lookup"><span data-stu-id="05e11-121">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="05e11-122">可取值为：`unknown`、`sender`、`recipient`。</span><span class="sxs-lookup"><span data-stu-id="05e11-122">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="05e11-123">isVpn</span><span class="sxs-lookup"><span data-stu-id="05e11-123">isVpn</span></span>|<span data-ttu-id="05e11-124">布尔值</span><span class="sxs-lookup"><span data-stu-id="05e11-124">Boolean</span></span>|<span data-ttu-id="05e11-125">指示用户是否通过 VPN 登录。</span><span class="sxs-lookup"><span data-stu-id="05e11-125">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="05e11-126">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="05e11-126">logonDateTime</span></span>|<span data-ttu-id="05e11-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05e11-127">DateTimeOffset</span></span>|<span data-ttu-id="05e11-128">登录发生的时间。</span><span class="sxs-lookup"><span data-stu-id="05e11-128">Time at which the sign-in occurred.</span></span> <span data-ttu-id="05e11-129">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="05e11-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="05e11-130">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="05e11-130">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="05e11-131">logonId</span><span class="sxs-lookup"><span data-stu-id="05e11-131">logonId</span></span>|<span data-ttu-id="05e11-132">String</span><span class="sxs-lookup"><span data-stu-id="05e11-132">String</span></span>|<span data-ttu-id="05e11-133">用户登录 ID。</span><span class="sxs-lookup"><span data-stu-id="05e11-133">User sign-in ID.</span></span>|
|<span data-ttu-id="05e11-134">logonIp</span><span class="sxs-lookup"><span data-stu-id="05e11-134">logonIp</span></span>|<span data-ttu-id="05e11-135">String</span><span class="sxs-lookup"><span data-stu-id="05e11-135">String</span></span>|<span data-ttu-id="05e11-136">IP 地址源自的登录请求。</span><span class="sxs-lookup"><span data-stu-id="05e11-136">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="05e11-137">logonLocation</span><span class="sxs-lookup"><span data-stu-id="05e11-137">logonLocation</span></span>|<span data-ttu-id="05e11-138">String</span><span class="sxs-lookup"><span data-stu-id="05e11-138">String</span></span>|<span data-ttu-id="05e11-139">位置 (与此) 登录事件关联的 IP 地址映射。</span><span class="sxs-lookup"><span data-stu-id="05e11-139">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="05e11-140">logonType</span><span class="sxs-lookup"><span data-stu-id="05e11-140">logonType</span></span>|<span data-ttu-id="05e11-141">logonType</span><span class="sxs-lookup"><span data-stu-id="05e11-141">logonType</span></span>|<span data-ttu-id="05e11-142">用户登录方法。</span><span class="sxs-lookup"><span data-stu-id="05e11-142">Method of user sign in.</span></span> <span data-ttu-id="05e11-143">可取值为：`unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。</span><span class="sxs-lookup"><span data-stu-id="05e11-143">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="05e11-144">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="05e11-144">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="05e11-145">String</span><span class="sxs-lookup"><span data-stu-id="05e11-145">String</span></span>|<span data-ttu-id="05e11-146">Active Directory (本地) 安全标识符 (SID) 用户的 SID。</span><span class="sxs-lookup"><span data-stu-id="05e11-146">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="05e11-147">riskScore</span><span class="sxs-lookup"><span data-stu-id="05e11-147">riskScore</span></span>|<span data-ttu-id="05e11-148">String</span><span class="sxs-lookup"><span data-stu-id="05e11-148">String</span></span>|<span data-ttu-id="05e11-149">用户帐户的提供程序生成/计算的风险评分。</span><span class="sxs-lookup"><span data-stu-id="05e11-149">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="05e11-150">建议的值范围为 0-1，等于百分比。</span><span class="sxs-lookup"><span data-stu-id="05e11-150">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="05e11-151">userAccountType</span><span class="sxs-lookup"><span data-stu-id="05e11-151">userAccountType</span></span>|<span data-ttu-id="05e11-152">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="05e11-152">userAccountSecurityType</span></span>|<span data-ttu-id="05e11-153">用户帐户类型 (Windows 定义) 组成员身份类型。</span><span class="sxs-lookup"><span data-stu-id="05e11-153">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="05e11-154">可取值为：`unknown`、`standard`、`power`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="05e11-154">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="05e11-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="05e11-155">userPrincipalName</span></span>|<span data-ttu-id="05e11-156">String</span><span class="sxs-lookup"><span data-stu-id="05e11-156">String</span></span>|<span data-ttu-id="05e11-157">用户登录名 - internet 格式： (用户帐户名称) @ (用户帐户 DNS 域名) 。</span><span class="sxs-lookup"><span data-stu-id="05e11-157">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="05e11-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="05e11-158">JSON representation</span></span>

<span data-ttu-id="05e11-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05e11-159">The following is a JSON representation of the resource.</span></span>

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


