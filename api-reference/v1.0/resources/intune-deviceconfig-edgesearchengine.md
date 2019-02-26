---
title: edgeSearchEngine 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6867dd6b2243541b193b8b741924487f16ff61c5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254469"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="34f1a-103">edgeSearchEngine 资源类型</span><span class="sxs-lookup"><span data-stu-id="34f1a-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="34f1a-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34f1a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34f1a-105">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="34f1a-105">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="34f1a-106">继承自 [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="34f1a-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="34f1a-107">属性</span><span class="sxs-lookup"><span data-stu-id="34f1a-107">Properties</span></span>
|<span data-ttu-id="34f1a-108">属性</span><span class="sxs-lookup"><span data-stu-id="34f1a-108">Property</span></span>|<span data-ttu-id="34f1a-109">类型</span><span class="sxs-lookup"><span data-stu-id="34f1a-109">Type</span></span>|<span data-ttu-id="34f1a-110">说明</span><span class="sxs-lookup"><span data-stu-id="34f1a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34f1a-111">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="34f1a-111">edgeSearchEngineType</span></span>|[<span data-ttu-id="34f1a-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="34f1a-112">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="34f1a-113">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="34f1a-113">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="34f1a-114">可取值为：`default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="34f1a-114">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34f1a-115">Relationships</span><span class="sxs-lookup"><span data-stu-id="34f1a-115">Relationships</span></span>
<span data-ttu-id="34f1a-116">无</span><span class="sxs-lookup"><span data-stu-id="34f1a-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34f1a-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="34f1a-117">JSON Representation</span></span>
<span data-ttu-id="34f1a-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34f1a-118">Here is a JSON representation of the resource.</span></span>
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



