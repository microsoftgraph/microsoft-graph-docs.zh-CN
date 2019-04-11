---
title: edgeSearchEngine 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 86604849a488f9f9bf8626f8bfba205efd11a532
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782763"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="a1f12-103">edgeSearchEngine 资源类型</span><span class="sxs-lookup"><span data-stu-id="a1f12-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="a1f12-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a1f12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1f12-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a1f12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1f12-106">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="a1f12-106">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="a1f12-107">继承自 [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="a1f12-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a1f12-108">属性</span><span class="sxs-lookup"><span data-stu-id="a1f12-108">Properties</span></span>
|<span data-ttu-id="a1f12-109">属性</span><span class="sxs-lookup"><span data-stu-id="a1f12-109">Property</span></span>|<span data-ttu-id="a1f12-110">类型</span><span class="sxs-lookup"><span data-stu-id="a1f12-110">Type</span></span>|<span data-ttu-id="a1f12-111">说明</span><span class="sxs-lookup"><span data-stu-id="a1f12-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1f12-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="a1f12-112">edgeSearchEngineType</span></span>|[<span data-ttu-id="a1f12-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="a1f12-113">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="a1f12-114">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="a1f12-114">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="a1f12-115">可取值为：`default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="a1f12-115">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1f12-116">关系</span><span class="sxs-lookup"><span data-stu-id="a1f12-116">Relationships</span></span>
<span data-ttu-id="a1f12-117">无</span><span class="sxs-lookup"><span data-stu-id="a1f12-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1f12-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a1f12-118">JSON Representation</span></span>
<span data-ttu-id="a1f12-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1f12-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngine"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngine",
  "edgeSearchEngineType": "String"
}
```





