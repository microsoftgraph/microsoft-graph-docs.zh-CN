---
title: edgeSearchEngineBase 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。 如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f2aeffb922ebf8b3a166b8f942d4159fa3fe7a3b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253321"
---
# <a name="edgesearchenginebase-resource-type"></a><span data-ttu-id="a7542-104">edgeSearchEngineBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="a7542-104">edgeSearchEngineBase resource type</span></span>

> <span data-ttu-id="a7542-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a7542-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7542-106">允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="a7542-106">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="a7542-107">如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="a7542-107">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>

## <a name="properties"></a><span data-ttu-id="a7542-108">属性</span><span class="sxs-lookup"><span data-stu-id="a7542-108">Properties</span></span>
|<span data-ttu-id="a7542-109">属性</span><span class="sxs-lookup"><span data-stu-id="a7542-109">Property</span></span>|<span data-ttu-id="a7542-110">类型</span><span class="sxs-lookup"><span data-stu-id="a7542-110">Type</span></span>|<span data-ttu-id="a7542-111">说明</span><span class="sxs-lookup"><span data-stu-id="a7542-111">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="a7542-112">关系</span><span class="sxs-lookup"><span data-stu-id="a7542-112">Relationships</span></span>
<span data-ttu-id="a7542-113">无</span><span class="sxs-lookup"><span data-stu-id="a7542-113">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7542-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a7542-114">JSON Representation</span></span>
<span data-ttu-id="a7542-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7542-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngineBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineBase"
}
```



