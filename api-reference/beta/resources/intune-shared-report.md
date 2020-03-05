---
title: report 资源类型
description: 介绍了适用于 Intune 的 Microsoft Graph API 的报告资源，它支持多个工作流。
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 22bb8cd564c4ad27f3299d193f5cea6ad3cbdf75
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523581"
---
# <a name="report-resource-type"></a><span data-ttu-id="1e4da-103">report 资源类型</span><span class="sxs-lookup"><span data-stu-id="1e4da-103">report resource type</span></span>

<span data-ttu-id="1e4da-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1e4da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1e4da-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1e4da-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e4da-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1e4da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e4da-107">返回适用于上下文的内容，包括：</span><span class="sxs-lookup"><span data-stu-id="1e4da-107">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="1e4da-108">设备配置文件历史记录报告。</span><span class="sxs-lookup"><span data-stu-id="1e4da-108">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="1e4da-109">注册失败报告。</span><span class="sxs-lookup"><span data-stu-id="1e4da-109">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="1e4da-110">属性</span><span class="sxs-lookup"><span data-stu-id="1e4da-110">Properties</span></span>
|<span data-ttu-id="1e4da-111">属性</span><span class="sxs-lookup"><span data-stu-id="1e4da-111">Property</span></span>|<span data-ttu-id="1e4da-112">类型</span><span class="sxs-lookup"><span data-stu-id="1e4da-112">Type</span></span>|<span data-ttu-id="1e4da-113">说明</span><span class="sxs-lookup"><span data-stu-id="1e4da-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e4da-114">content</span><span class="sxs-lookup"><span data-stu-id="1e4da-114">content</span></span>|<span data-ttu-id="1e4da-115">流</span><span class="sxs-lookup"><span data-stu-id="1e4da-115">Stream</span></span>|<span data-ttu-id="1e4da-116">报告内容;详细信息因报告类型而异。</span><span class="sxs-lookup"><span data-stu-id="1e4da-116">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e4da-117">关系</span><span class="sxs-lookup"><span data-stu-id="1e4da-117">Relationships</span></span>
<span data-ttu-id="1e4da-118">无</span><span class="sxs-lookup"><span data-stu-id="1e4da-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e4da-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1e4da-119">JSON Representation</span></span>
<span data-ttu-id="1e4da-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e4da-120">Here is a JSON representation of the resource.</span></span>
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



