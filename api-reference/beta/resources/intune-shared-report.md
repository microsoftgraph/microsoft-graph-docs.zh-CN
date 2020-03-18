---
title: report 资源类型
description: 介绍了适用于 Intune 的 Microsoft Graph API 的报告资源，它支持多个工作流。
localization_priority: Normal
author: davidmu1
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d321b5a2dadc4a459194a24224805f7443592532
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42768007"
---
# <a name="report-resource-type"></a><span data-ttu-id="dece7-103">report 资源类型</span><span class="sxs-lookup"><span data-stu-id="dece7-103">report resource type</span></span>

> <span data-ttu-id="dece7-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dece7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dece7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dece7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dece7-106">返回适用于上下文的内容，包括：</span><span class="sxs-lookup"><span data-stu-id="dece7-106">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="dece7-107">设备配置文件历史记录报告。</span><span class="sxs-lookup"><span data-stu-id="dece7-107">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="dece7-108">注册失败报告。</span><span class="sxs-lookup"><span data-stu-id="dece7-108">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="dece7-109">属性</span><span class="sxs-lookup"><span data-stu-id="dece7-109">Properties</span></span>
|<span data-ttu-id="dece7-110">属性</span><span class="sxs-lookup"><span data-stu-id="dece7-110">Property</span></span>|<span data-ttu-id="dece7-111">类型</span><span class="sxs-lookup"><span data-stu-id="dece7-111">Type</span></span>|<span data-ttu-id="dece7-112">说明</span><span class="sxs-lookup"><span data-stu-id="dece7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dece7-113">content</span><span class="sxs-lookup"><span data-stu-id="dece7-113">content</span></span>|<span data-ttu-id="dece7-114">流</span><span class="sxs-lookup"><span data-stu-id="dece7-114">Stream</span></span>|<span data-ttu-id="dece7-115">报告内容;详细信息因报告类型而异。</span><span class="sxs-lookup"><span data-stu-id="dece7-115">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dece7-116">关系</span><span class="sxs-lookup"><span data-stu-id="dece7-116">Relationships</span></span>
<span data-ttu-id="dece7-117">无</span><span class="sxs-lookup"><span data-stu-id="dece7-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dece7-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dece7-118">JSON Representation</span></span>
<span data-ttu-id="dece7-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dece7-119">Here is a JSON representation of the resource.</span></span>
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



