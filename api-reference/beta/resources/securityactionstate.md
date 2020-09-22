---
title: securityActionState 资源类型
description: 表示 securityAction 状态更改的历史记录。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: ba22a03f4d4a6d03b0093ed28b8c54a7c095d037
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988861"
---
# <a name="securityactionstate-resource-type"></a><span data-ttu-id="eba15-103">securityActionState 资源类型</span><span class="sxs-lookup"><span data-stu-id="eba15-103">securityActionState resource type</span></span>

<span data-ttu-id="eba15-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eba15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eba15-105">表示 securityAction 状态更改的历史记录。</span><span class="sxs-lookup"><span data-stu-id="eba15-105">Represents the history of securityAction state changes.</span></span>

## <a name="properties"></a><span data-ttu-id="eba15-106">属性</span><span class="sxs-lookup"><span data-stu-id="eba15-106">Properties</span></span>

| <span data-ttu-id="eba15-107">属性</span><span class="sxs-lookup"><span data-stu-id="eba15-107">Property</span></span>     | <span data-ttu-id="eba15-108">类型</span><span class="sxs-lookup"><span data-stu-id="eba15-108">Type</span></span>        | <span data-ttu-id="eba15-109">说明</span><span class="sxs-lookup"><span data-stu-id="eba15-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eba15-110">appId</span><span class="sxs-lookup"><span data-stu-id="eba15-110">appId</span></span>|<span data-ttu-id="eba15-111">String</span><span class="sxs-lookup"><span data-stu-id="eba15-111">String</span></span>|<span data-ttu-id="eba15-112">向操作提交更新 (PATCH) 的调用应用程序的应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="eba15-112">The Application ID of the calling application that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="eba15-113">`appId`应从 auth 令牌中提取，而不是通过调用应用程序手动输入。</span><span class="sxs-lookup"><span data-stu-id="eba15-113">The `appId` should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="eba15-114">状态</span><span class="sxs-lookup"><span data-stu-id="eba15-114">status</span></span>|<span data-ttu-id="eba15-115">String</span><span class="sxs-lookup"><span data-stu-id="eba15-115">String</span></span>| <span data-ttu-id="eba15-116">此更新中的 securityAction 的状态。</span><span class="sxs-lookup"><span data-stu-id="eba15-116">Status of the securityAction in this update.</span></span> <span data-ttu-id="eba15-117">可取值为：`NotStarted`、`Running`、`Completed`、`Failed`。</span><span class="sxs-lookup"><span data-stu-id="eba15-117">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="eba15-118">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="eba15-118">updatedDateTime</span></span>|<span data-ttu-id="eba15-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eba15-119">DateTimeOffset</span></span>| <span data-ttu-id="eba15-120">更新 actionState 时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="eba15-120">Timestamp when the actionState was updated.</span></span> <span data-ttu-id="eba15-121">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="eba15-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="eba15-122">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="eba15-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="eba15-123">user</span><span class="sxs-lookup"><span data-stu-id="eba15-123">user</span></span>|<span data-ttu-id="eba15-124">String</span><span class="sxs-lookup"><span data-stu-id="eba15-124">String</span></span>|<span data-ttu-id="eba15-125">向操作提交更新 (PATCH) 的已登录用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="eba15-125">The user principal name of the signed-in user that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="eba15-126">`user`应从 auth 令牌中提取，而不是通过调用应用程序手动输入。</span><span class="sxs-lookup"><span data-stu-id="eba15-126">The `user` should be extracted from the auth token and not entered manually by the calling application.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eba15-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eba15-127">JSON representation</span></span>

<span data-ttu-id="eba15-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eba15-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityActionState",
  "baseType": null
}-->

```json
{
  "appId": "String",
  "status": "String",
  "updatedDateTime": "String (timestamp)",
  "user": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityActionState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


