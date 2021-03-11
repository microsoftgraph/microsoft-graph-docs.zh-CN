---
title: logonUser 资源类型
description: 包含有关此主机上已登录用户的有状态信息
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 9986aaa7cb5fbf5f8687c43de019b234a4a971d8
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720492"
---
# <a name="logonuser-resource-type"></a><span data-ttu-id="e2356-103">logonUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2356-103">logonUser resource type</span></span>

<span data-ttu-id="e2356-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2356-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e2356-105">包含有关此主机上已登录用户的有状态信息</span><span class="sxs-lookup"><span data-stu-id="e2356-105">Contains stateful information about the logged on user on this host</span></span>

## <a name="properties"></a><span data-ttu-id="e2356-106">属性</span><span class="sxs-lookup"><span data-stu-id="e2356-106">Properties</span></span>

| <span data-ttu-id="e2356-107">属性</span><span class="sxs-lookup"><span data-stu-id="e2356-107">Property</span></span>   | <span data-ttu-id="e2356-108">类型</span><span class="sxs-lookup"><span data-stu-id="e2356-108">Type</span></span> |<span data-ttu-id="e2356-109">说明</span><span class="sxs-lookup"><span data-stu-id="e2356-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2356-110">accountDomain</span><span class="sxs-lookup"><span data-stu-id="e2356-110">accountDomain</span></span>|<span data-ttu-id="e2356-111">String</span><span class="sxs-lookup"><span data-stu-id="e2356-111">String</span></span>|<span data-ttu-id="e2356-112">用于登录的用户帐户的域。</span><span class="sxs-lookup"><span data-stu-id="e2356-112">Domain of user account used to logon.</span></span>|
|<span data-ttu-id="e2356-113">accountName</span><span class="sxs-lookup"><span data-stu-id="e2356-113">accountName</span></span>|<span data-ttu-id="e2356-114">String</span><span class="sxs-lookup"><span data-stu-id="e2356-114">String</span></span>|<span data-ttu-id="e2356-115">用于登录的用户帐户的帐户名称。</span><span class="sxs-lookup"><span data-stu-id="e2356-115">Account name of user account used to logon.</span></span>|
|<span data-ttu-id="e2356-116">accountType</span><span class="sxs-lookup"><span data-stu-id="e2356-116">accountType</span></span>|<span data-ttu-id="e2356-117">String</span><span class="sxs-lookup"><span data-stu-id="e2356-117">String</span></span>|<span data-ttu-id="e2356-118">用户帐户类型（按 Windows 定义）。</span><span class="sxs-lookup"><span data-stu-id="e2356-118">User Account type, per Windows definition.</span></span> <span data-ttu-id="e2356-119">可取值为：`unknown`、`standard`、`power`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="e2356-119">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="e2356-120">firstSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="e2356-120">firstSeenDateTime</span></span>|<span data-ttu-id="e2356-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2356-121">DateTimeOffset</span></span>|<span data-ttu-id="e2356-122">此用户帐户最早登录的日期/时间 (提供程序确定的) 。</span><span class="sxs-lookup"><span data-stu-id="e2356-122">DateTime at which the earliest logon by this user account occurred (provider-determined period).</span></span> <span data-ttu-id="e2356-123">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="e2356-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e2356-124">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="e2356-124">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="e2356-125">lastSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="e2356-125">lastSeenDateTime</span></span>|<span data-ttu-id="e2356-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2356-126">DateTimeOffset</span></span>|<span data-ttu-id="e2356-127">发生此用户帐户最新登录的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e2356-127">DateTime at which the latest logon by this user account occurred.</span></span> <span data-ttu-id="e2356-128">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="e2356-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e2356-129">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="e2356-129">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="e2356-130">logonId</span><span class="sxs-lookup"><span data-stu-id="e2356-130">logonId</span></span>|<span data-ttu-id="e2356-131">String</span><span class="sxs-lookup"><span data-stu-id="e2356-131">String</span></span>|<span data-ttu-id="e2356-132">用户登录 ID。</span><span class="sxs-lookup"><span data-stu-id="e2356-132">User logon ID.</span></span>|
|<span data-ttu-id="e2356-133">logonTypes</span><span class="sxs-lookup"><span data-stu-id="e2356-133">logonTypes</span></span>|<span data-ttu-id="e2356-134">字符串集合</span><span class="sxs-lookup"><span data-stu-id="e2356-134">String collection</span></span>|<span data-ttu-id="e2356-135">从首次看到到最后一次看到时为登录用户观察到的登录类型的集合。</span><span class="sxs-lookup"><span data-stu-id="e2356-135">Collection of the logon types observed for the logged on user from when first to last seen.</span></span> <span data-ttu-id="e2356-136">可取值为：`unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。</span><span class="sxs-lookup"><span data-stu-id="e2356-136">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2356-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2356-137">JSON representation</span></span>

<span data-ttu-id="e2356-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2356-138">The following is a JSON representation of the resource.</span></span>

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


