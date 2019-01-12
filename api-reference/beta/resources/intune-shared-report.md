---
title: report 资源类型
description: 将内容返回相应的上下文中，包括：
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: dbad8a8808d40c2ae1f7769773b6b29ef65d680f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970645"
---
# <a name="report-resource-type"></a><span data-ttu-id="f1eb0-103">report 资源类型</span><span class="sxs-lookup"><span data-stu-id="f1eb0-103">report resource type</span></span>

> <span data-ttu-id="f1eb0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f1eb0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1eb0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f1eb0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1eb0-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f1eb0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1eb0-107">将内容返回相应的上下文中，包括：</span><span class="sxs-lookup"><span data-stu-id="f1eb0-107">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="f1eb0-108">设备配置配置文件历史记录的报告。</span><span class="sxs-lookup"><span data-stu-id="f1eb0-108">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="f1eb0-109">注册失败报告。</span><span class="sxs-lookup"><span data-stu-id="f1eb0-109">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="f1eb0-110">属性</span><span class="sxs-lookup"><span data-stu-id="f1eb0-110">Properties</span></span>
|<span data-ttu-id="f1eb0-111">属性</span><span class="sxs-lookup"><span data-stu-id="f1eb0-111">Property</span></span>|<span data-ttu-id="f1eb0-112">类型</span><span class="sxs-lookup"><span data-stu-id="f1eb0-112">Type</span></span>|<span data-ttu-id="f1eb0-113">说明</span><span class="sxs-lookup"><span data-stu-id="f1eb0-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1eb0-114">内容</span><span class="sxs-lookup"><span data-stu-id="f1eb0-114">content</span></span>|<span data-ttu-id="f1eb0-115">Stream</span><span class="sxs-lookup"><span data-stu-id="f1eb0-115">Stream</span></span>|<span data-ttu-id="f1eb0-116">报表内容;因报表类型而异详细信息。</span><span class="sxs-lookup"><span data-stu-id="f1eb0-116">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1eb0-117">Relationships</span><span class="sxs-lookup"><span data-stu-id="f1eb0-117">Relationships</span></span>
<span data-ttu-id="f1eb0-118">无</span><span class="sxs-lookup"><span data-stu-id="f1eb0-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1eb0-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1eb0-119">JSON Representation</span></span>
<span data-ttu-id="f1eb0-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1eb0-120">Here is a JSON representation of the resource.</span></span>
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



