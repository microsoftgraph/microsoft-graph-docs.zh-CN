---
title: logonUser 资源类型
description: 包含有关在用户登录该主机上的状态信息
localization_priority: Normal
ms.openlocfilehash: 3b7862555c62eb16aaceaa53d4df58541426e08a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855592"
---
# <a name="logonuser-resource-type"></a><span data-ttu-id="1fe4a-103">logonUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="1fe4a-103">logonUser resource type</span></span>

<span data-ttu-id="1fe4a-104">包含有关在用户登录该主机上的状态信息</span><span class="sxs-lookup"><span data-stu-id="1fe4a-104">Contains stateful information about the logged on user on this host</span></span>

## <a name="properties"></a><span data-ttu-id="1fe4a-105">属性</span><span class="sxs-lookup"><span data-stu-id="1fe4a-105">Properties</span></span>

| <span data-ttu-id="1fe4a-106">属性</span><span class="sxs-lookup"><span data-stu-id="1fe4a-106">Property</span></span>   | <span data-ttu-id="1fe4a-107">类型</span><span class="sxs-lookup"><span data-stu-id="1fe4a-107">Type</span></span> |<span data-ttu-id="1fe4a-108">Description</span><span class="sxs-lookup"><span data-stu-id="1fe4a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1fe4a-109">accountDomain</span><span class="sxs-lookup"><span data-stu-id="1fe4a-109">accountDomain</span></span>|<span data-ttu-id="1fe4a-110">字符串</span><span class="sxs-lookup"><span data-stu-id="1fe4a-110">String</span></span>|<span data-ttu-id="1fe4a-111">域使用的用户帐户登录。</span><span class="sxs-lookup"><span data-stu-id="1fe4a-111">Domain of user account used to logon.</span></span>|
|<span data-ttu-id="1fe4a-112">accountName</span><span class="sxs-lookup"><span data-stu-id="1fe4a-112">accountName</span></span>|<span data-ttu-id="1fe4a-113">字符串</span><span class="sxs-lookup"><span data-stu-id="1fe4a-113">String</span></span>|<span data-ttu-id="1fe4a-114">使用的用户帐户的帐户名称为登录。</span><span class="sxs-lookup"><span data-stu-id="1fe4a-114">Account name of user account used to logon.</span></span>|
|<span data-ttu-id="1fe4a-115">accountType</span><span class="sxs-lookup"><span data-stu-id="1fe4a-115">accountType</span></span>|<span data-ttu-id="1fe4a-116">字符串</span><span class="sxs-lookup"><span data-stu-id="1fe4a-116">String</span></span>|<span data-ttu-id="1fe4a-117">用户帐户类型，每 Windows 定义。</span><span class="sxs-lookup"><span data-stu-id="1fe4a-117">User Account type, per Windows definition.</span></span> <span data-ttu-id="1fe4a-118">可取值为：`unknown`、`standard`、`power`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="1fe4a-118">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="1fe4a-119">firstSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="1fe4a-119">firstSeenDateTime</span></span>|<span data-ttu-id="1fe4a-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1fe4a-120">DateTimeOffset</span></span>|<span data-ttu-id="1fe4a-121">最早登录该用户帐户的发生的日期时间 （提供程序确定期间）。</span><span class="sxs-lookup"><span data-stu-id="1fe4a-121">DateTime at which the earliest logon by this user account occurred (provider-determined period).</span></span> <span data-ttu-id="1fe4a-122">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="1fe4a-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1fe4a-123">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="1fe4a-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="1fe4a-124">lastSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="1fe4a-124">lastSeenDateTime</span></span>|<span data-ttu-id="1fe4a-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1fe4a-125">DateTimeOffset</span></span>|<span data-ttu-id="1fe4a-126">通过此用户帐户的最新登录的发生的日期时间。</span><span class="sxs-lookup"><span data-stu-id="1fe4a-126">DateTime at which the latest logon by this user account occurred.</span></span> <span data-ttu-id="1fe4a-127">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="1fe4a-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1fe4a-128">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="1fe4a-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="1fe4a-129">logonId</span><span class="sxs-lookup"><span data-stu-id="1fe4a-129">logonId</span></span>|<span data-ttu-id="1fe4a-130">字符串</span><span class="sxs-lookup"><span data-stu-id="1fe4a-130">String</span></span>|<span data-ttu-id="1fe4a-131">用户登录 id。</span><span class="sxs-lookup"><span data-stu-id="1fe4a-131">User logon ID.</span></span>|
|<span data-ttu-id="1fe4a-132">logonTypes</span><span class="sxs-lookup"><span data-stu-id="1fe4a-132">logonTypes</span></span>|<span data-ttu-id="1fe4a-133">String 集合</span><span class="sxs-lookup"><span data-stu-id="1fe4a-133">String collection</span></span>|<span data-ttu-id="1fe4a-134">当一到最后一个发现观察的登录用户的登录类型的集合。</span><span class="sxs-lookup"><span data-stu-id="1fe4a-134">Collection of the logon types observed for the logged on user from when first to last seen.</span></span> <span data-ttu-id="1fe4a-135">可取值为：`unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。</span><span class="sxs-lookup"><span data-stu-id="1fe4a-135">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1fe4a-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1fe4a-136">JSON representation</span></span>

<span data-ttu-id="1fe4a-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1fe4a-137">The following is a JSON representation of the resource.</span></span>

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
