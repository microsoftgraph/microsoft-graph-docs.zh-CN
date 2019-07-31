---
title: securityActionState 资源类型
description: 表示 securityAction 状态更改的历史记录。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: e3efd29e156b6e0346574c74fad2a30a39ec7131
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008507"
---
# <a name="securityactionstate-resource-type"></a><span data-ttu-id="2e8bb-103">securityActionState 资源类型</span><span class="sxs-lookup"><span data-stu-id="2e8bb-103">securityActionState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e8bb-104">表示 securityAction 状态更改的历史记录。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-104">Represents the history of securityAction state changes.</span></span>

## <a name="properties"></a><span data-ttu-id="2e8bb-105">属性</span><span class="sxs-lookup"><span data-stu-id="2e8bb-105">Properties</span></span>

| <span data-ttu-id="2e8bb-106">属性</span><span class="sxs-lookup"><span data-stu-id="2e8bb-106">Property</span></span>     | <span data-ttu-id="2e8bb-107">类型</span><span class="sxs-lookup"><span data-stu-id="2e8bb-107">Type</span></span>        | <span data-ttu-id="2e8bb-108">说明</span><span class="sxs-lookup"><span data-stu-id="2e8bb-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2e8bb-109">appId</span><span class="sxs-lookup"><span data-stu-id="2e8bb-109">appId</span></span>|<span data-ttu-id="2e8bb-110">String</span><span class="sxs-lookup"><span data-stu-id="2e8bb-110">String</span></span>|<span data-ttu-id="2e8bb-111">向操作提交更新 (修补程序) 的呼叫应用程序的应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-111">The Application ID of the calling application that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="2e8bb-112">`appId`应从 auth 令牌中提取, 而不是通过调用应用程序手动输入。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-112">The `appId` should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="2e8bb-113">status</span><span class="sxs-lookup"><span data-stu-id="2e8bb-113">status</span></span>|<span data-ttu-id="2e8bb-114">String</span><span class="sxs-lookup"><span data-stu-id="2e8bb-114">String</span></span>| <span data-ttu-id="2e8bb-115">此更新中的 securityAction 的状态。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-115">Status of the securityAction in this update.</span></span> <span data-ttu-id="2e8bb-116">可取值为：`NotStarted`、`Running`、`Completed`、`Failed`。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-116">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="2e8bb-117">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e8bb-117">updatedDateTime</span></span>|<span data-ttu-id="2e8bb-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e8bb-118">DateTimeOffset</span></span>| <span data-ttu-id="2e8bb-119">更新 actionState 时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-119">Timestamp when the actionState was updated.</span></span> <span data-ttu-id="2e8bb-120">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2e8bb-121">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2e8bb-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2e8bb-122">user</span><span class="sxs-lookup"><span data-stu-id="2e8bb-122">user</span></span>|<span data-ttu-id="2e8bb-123">String</span><span class="sxs-lookup"><span data-stu-id="2e8bb-123">String</span></span>|<span data-ttu-id="2e8bb-124">向操作提交更新 (修补程序) 的已登录用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-124">The user principal name of the signed-in user that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="2e8bb-125">`user`应从 auth 令牌中提取, 而不是通过调用应用程序手动输入。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-125">The `user` should be extracted from the auth token and not entered manually by the calling application.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2e8bb-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2e8bb-126">JSON representation</span></span>

<span data-ttu-id="2e8bb-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-127">The following is a JSON representation of the resource.</span></span>

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
