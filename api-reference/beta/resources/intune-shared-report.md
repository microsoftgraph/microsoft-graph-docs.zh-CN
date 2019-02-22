---
title: report 资源类型
description: 介绍了适用于 Intune 的 Microsoft Graph API 的报告资源, 它支持多个工作流。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: f523f6df0b8b90cb6649ac81f1e433d6df227aea
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165749"
---
# <a name="report-resource-type"></a><span data-ttu-id="b781d-103">report 资源类型</span><span class="sxs-lookup"><span data-stu-id="b781d-103">report resource type</span></span>

> <span data-ttu-id="b781d-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b781d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b781d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b781d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b781d-106">返回适用于上下文的内容, 包括:</span><span class="sxs-lookup"><span data-stu-id="b781d-106">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="b781d-107">设备配置文件历史记录报告。</span><span class="sxs-lookup"><span data-stu-id="b781d-107">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="b781d-108">注册失败报告。</span><span class="sxs-lookup"><span data-stu-id="b781d-108">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="b781d-109">属性</span><span class="sxs-lookup"><span data-stu-id="b781d-109">Properties</span></span>
|<span data-ttu-id="b781d-110">属性</span><span class="sxs-lookup"><span data-stu-id="b781d-110">Property</span></span>|<span data-ttu-id="b781d-111">类型</span><span class="sxs-lookup"><span data-stu-id="b781d-111">Type</span></span>|<span data-ttu-id="b781d-112">说明</span><span class="sxs-lookup"><span data-stu-id="b781d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b781d-113">内容</span><span class="sxs-lookup"><span data-stu-id="b781d-113">content</span></span>|<span data-ttu-id="b781d-114">Stream</span><span class="sxs-lookup"><span data-stu-id="b781d-114">Stream</span></span>|<span data-ttu-id="b781d-115">报告内容;详细信息因报告类型而异。</span><span class="sxs-lookup"><span data-stu-id="b781d-115">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b781d-116">关系</span><span class="sxs-lookup"><span data-stu-id="b781d-116">Relationships</span></span>
<span data-ttu-id="b781d-117">无</span><span class="sxs-lookup"><span data-stu-id="b781d-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b781d-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b781d-118">JSON Representation</span></span>
<span data-ttu-id="b781d-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b781d-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.report"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.report",
  "content": "<Unknown Primitive Type Edm.Stream>"
}
```



