---
title: deviceActionResult 资源类型
description: 设备操作结果
ms.openlocfilehash: 9d7804b994474778f0f06c52079e09ed5887a09f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010426"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="26acb-103">deviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="26acb-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="26acb-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="26acb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26acb-105">设备操作结果</span><span class="sxs-lookup"><span data-stu-id="26acb-105">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="26acb-106">属性</span><span class="sxs-lookup"><span data-stu-id="26acb-106">Properties</span></span>
|<span data-ttu-id="26acb-107">属性</span><span class="sxs-lookup"><span data-stu-id="26acb-107">Property</span></span>|<span data-ttu-id="26acb-108">类型</span><span class="sxs-lookup"><span data-stu-id="26acb-108">Type</span></span>|<span data-ttu-id="26acb-109">说明</span><span class="sxs-lookup"><span data-stu-id="26acb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26acb-110">actionName</span><span class="sxs-lookup"><span data-stu-id="26acb-110">actionName</span></span>|<span data-ttu-id="26acb-111">String</span><span class="sxs-lookup"><span data-stu-id="26acb-111">String</span></span>|<span data-ttu-id="26acb-112">操作名</span><span class="sxs-lookup"><span data-stu-id="26acb-112">Action name</span></span>|
|<span data-ttu-id="26acb-113">actionState</span><span class="sxs-lookup"><span data-stu-id="26acb-113">actionState</span></span>|[<span data-ttu-id="26acb-114">actionState</span><span class="sxs-lookup"><span data-stu-id="26acb-114">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="26acb-115">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="26acb-115">State of the action.</span></span> <span data-ttu-id="26acb-116">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="26acb-116">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="26acb-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="26acb-117">startDateTime</span></span>|<span data-ttu-id="26acb-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26acb-118">DateTimeOffset</span></span>|<span data-ttu-id="26acb-119">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="26acb-119">Time the action was initiated</span></span>|
|<span data-ttu-id="26acb-120">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="26acb-120">lastUpdatedDateTime</span></span>|<span data-ttu-id="26acb-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26acb-121">DateTimeOffset</span></span>|<span data-ttu-id="26acb-122">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="26acb-122">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="26acb-123">关系</span><span class="sxs-lookup"><span data-stu-id="26acb-123">Relationships</span></span>
<span data-ttu-id="26acb-124">无</span><span class="sxs-lookup"><span data-stu-id="26acb-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="26acb-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26acb-125">JSON Representation</span></span>
<span data-ttu-id="26acb-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26acb-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```



