---
title: logonUser 资源类型
description: 包含有关此主机上登录的用户的状态信息
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: f480ff8c67c602512d7d8ef3f090366734f0ca7e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808660"
---
# <a name="logonuser-resource-type"></a><span data-ttu-id="ee314-103">logonUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="ee314-103">logonUser resource type</span></span>

<span data-ttu-id="ee314-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee314-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ee314-105">包含有关此主机上登录的用户的状态信息</span><span class="sxs-lookup"><span data-stu-id="ee314-105">Contains stateful information about the logged on user on this host</span></span>

## <a name="properties"></a><span data-ttu-id="ee314-106">属性</span><span class="sxs-lookup"><span data-stu-id="ee314-106">Properties</span></span>

| <span data-ttu-id="ee314-107">属性</span><span class="sxs-lookup"><span data-stu-id="ee314-107">Property</span></span>   | <span data-ttu-id="ee314-108">类型</span><span class="sxs-lookup"><span data-stu-id="ee314-108">Type</span></span> |<span data-ttu-id="ee314-109">说明</span><span class="sxs-lookup"><span data-stu-id="ee314-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee314-110">accountDomain</span><span class="sxs-lookup"><span data-stu-id="ee314-110">accountDomain</span></span>|<span data-ttu-id="ee314-111">String</span><span class="sxs-lookup"><span data-stu-id="ee314-111">String</span></span>|<span data-ttu-id="ee314-112">用于登录的用户帐户的域。</span><span class="sxs-lookup"><span data-stu-id="ee314-112">Domain of user account used to logon.</span></span>|
|<span data-ttu-id="ee314-113">帐户</span><span class="sxs-lookup"><span data-stu-id="ee314-113">accountName</span></span>|<span data-ttu-id="ee314-114">String</span><span class="sxs-lookup"><span data-stu-id="ee314-114">String</span></span>|<span data-ttu-id="ee314-115">用于登录的用户帐户的帐户名。</span><span class="sxs-lookup"><span data-stu-id="ee314-115">Account name of user account used to logon.</span></span>|
|<span data-ttu-id="ee314-116">accountType</span><span class="sxs-lookup"><span data-stu-id="ee314-116">accountType</span></span>|<span data-ttu-id="ee314-117">String</span><span class="sxs-lookup"><span data-stu-id="ee314-117">String</span></span>|<span data-ttu-id="ee314-118">每个 Windows 定义的用户帐户类型。</span><span class="sxs-lookup"><span data-stu-id="ee314-118">User Account type, per Windows definition.</span></span> <span data-ttu-id="ee314-119">可取值为：`unknown`、`standard`、`power`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="ee314-119">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="ee314-120">firstSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="ee314-120">firstSeenDateTime</span></span>|<span data-ttu-id="ee314-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee314-121">DateTimeOffset</span></span>|<span data-ttu-id="ee314-122">按此用户帐户的最早登录发生的日期时间 (提供程序确定的时间段) 。</span><span class="sxs-lookup"><span data-stu-id="ee314-122">DateTime at which the earliest logon by this user account occurred (provider-determined period).</span></span> <span data-ttu-id="ee314-123">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="ee314-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ee314-124">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="ee314-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="ee314-125">lastSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="ee314-125">lastSeenDateTime</span></span>|<span data-ttu-id="ee314-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee314-126">DateTimeOffset</span></span>|<span data-ttu-id="ee314-127">发生此用户帐户的最新登录的日期时间。</span><span class="sxs-lookup"><span data-stu-id="ee314-127">DateTime at which the latest logon by this user account occurred.</span></span> <span data-ttu-id="ee314-128">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="ee314-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ee314-129">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="ee314-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="ee314-130">logonId</span><span class="sxs-lookup"><span data-stu-id="ee314-130">logonId</span></span>|<span data-ttu-id="ee314-131">String</span><span class="sxs-lookup"><span data-stu-id="ee314-131">String</span></span>|<span data-ttu-id="ee314-132">用户登录 ID。</span><span class="sxs-lookup"><span data-stu-id="ee314-132">User logon ID.</span></span>|
|<span data-ttu-id="ee314-133">了 logontypes</span><span class="sxs-lookup"><span data-stu-id="ee314-133">logonTypes</span></span>|<span data-ttu-id="ee314-134">字符串集合</span><span class="sxs-lookup"><span data-stu-id="ee314-134">String collection</span></span>|<span data-ttu-id="ee314-135">从第一次查看之时开始，登录用户看到的登录类型的集合。</span><span class="sxs-lookup"><span data-stu-id="ee314-135">Collection of the logon types observed for the logged on user from when first to last seen.</span></span> <span data-ttu-id="ee314-136">可取值为：`unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。</span><span class="sxs-lookup"><span data-stu-id="ee314-136">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ee314-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee314-137">JSON representation</span></span>

<span data-ttu-id="ee314-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee314-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.logonUser"
}-->

```json
{
  "accountDomain": "String",
  "accountName": "String",
  "accountType": "String",
  "firstSeenDateTime": "String (timestamp)",
  "lastSeenDateTime": "String (timestamp)",
  "logonId": "String",
  "logonTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "logonUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
