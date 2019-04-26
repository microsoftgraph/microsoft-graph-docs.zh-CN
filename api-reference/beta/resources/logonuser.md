---
title: logonUser 资源类型
description: 包含有关此主机上登录的用户的状态信息
localization_priority: Normal
ms.openlocfilehash: 3b7862555c62eb16aaceaa53d4df58541426e08a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562655"
---
# <a name="logonuser-resource-type"></a><span data-ttu-id="327ec-103">logonUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="327ec-103">logonUser resource type</span></span>

<span data-ttu-id="327ec-104">包含有关此主机上登录的用户的状态信息</span><span class="sxs-lookup"><span data-stu-id="327ec-104">Contains stateful information about the logged on user on this host</span></span>

## <a name="properties"></a><span data-ttu-id="327ec-105">属性</span><span class="sxs-lookup"><span data-stu-id="327ec-105">Properties</span></span>

| <span data-ttu-id="327ec-106">属性</span><span class="sxs-lookup"><span data-stu-id="327ec-106">Property</span></span>   | <span data-ttu-id="327ec-107">类型</span><span class="sxs-lookup"><span data-stu-id="327ec-107">Type</span></span> |<span data-ttu-id="327ec-108">说明</span><span class="sxs-lookup"><span data-stu-id="327ec-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="327ec-109">accountDomain</span><span class="sxs-lookup"><span data-stu-id="327ec-109">accountDomain</span></span>|<span data-ttu-id="327ec-110">String</span><span class="sxs-lookup"><span data-stu-id="327ec-110">String</span></span>|<span data-ttu-id="327ec-111">用于登录的用户帐户的域。</span><span class="sxs-lookup"><span data-stu-id="327ec-111">Domain of user account used to logon.</span></span>|
|<span data-ttu-id="327ec-112">帐户</span><span class="sxs-lookup"><span data-stu-id="327ec-112">accountName</span></span>|<span data-ttu-id="327ec-113">String</span><span class="sxs-lookup"><span data-stu-id="327ec-113">String</span></span>|<span data-ttu-id="327ec-114">用于登录的用户帐户的帐户名。</span><span class="sxs-lookup"><span data-stu-id="327ec-114">Account name of user account used to logon.</span></span>|
|<span data-ttu-id="327ec-115">accountType</span><span class="sxs-lookup"><span data-stu-id="327ec-115">accountType</span></span>|<span data-ttu-id="327ec-116">String</span><span class="sxs-lookup"><span data-stu-id="327ec-116">String</span></span>|<span data-ttu-id="327ec-117">每个 Windows 定义的用户帐户类型。</span><span class="sxs-lookup"><span data-stu-id="327ec-117">User Account type, per Windows definition.</span></span> <span data-ttu-id="327ec-118">可取值为：`unknown`、`standard`、`power`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="327ec-118">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="327ec-119">firstSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="327ec-119">firstSeenDateTime</span></span>|<span data-ttu-id="327ec-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="327ec-120">DateTimeOffset</span></span>|<span data-ttu-id="327ec-121">发生此用户帐户的最早登录 (由提供程序确定的时间段) 的日期时间。</span><span class="sxs-lookup"><span data-stu-id="327ec-121">DateTime at which the earliest logon by this user account occurred (provider-determined period).</span></span> <span data-ttu-id="327ec-122">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="327ec-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="327ec-123">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="327ec-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="327ec-124">lastSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="327ec-124">lastSeenDateTime</span></span>|<span data-ttu-id="327ec-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="327ec-125">DateTimeOffset</span></span>|<span data-ttu-id="327ec-126">发生此用户帐户的最新登录的日期时间。</span><span class="sxs-lookup"><span data-stu-id="327ec-126">DateTime at which the latest logon by this user account occurred.</span></span> <span data-ttu-id="327ec-127">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="327ec-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="327ec-128">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="327ec-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="327ec-129">logonId</span><span class="sxs-lookup"><span data-stu-id="327ec-129">logonId</span></span>|<span data-ttu-id="327ec-130">String</span><span class="sxs-lookup"><span data-stu-id="327ec-130">String</span></span>|<span data-ttu-id="327ec-131">用户登录 ID。</span><span class="sxs-lookup"><span data-stu-id="327ec-131">User logon ID.</span></span>|
|<span data-ttu-id="327ec-132">了 logontypes</span><span class="sxs-lookup"><span data-stu-id="327ec-132">logonTypes</span></span>|<span data-ttu-id="327ec-133">String collection</span><span class="sxs-lookup"><span data-stu-id="327ec-133">String collection</span></span>|<span data-ttu-id="327ec-134">从第一次查看之时开始, 登录用户看到的登录类型的集合。</span><span class="sxs-lookup"><span data-stu-id="327ec-134">Collection of the logon types observed for the logged on user from when first to last seen.</span></span> <span data-ttu-id="327ec-135">可取值为：`unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。</span><span class="sxs-lookup"><span data-stu-id="327ec-135">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="327ec-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="327ec-136">JSON representation</span></span>

<span data-ttu-id="327ec-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="327ec-137">The following is a JSON representation of the resource.</span></span>

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
