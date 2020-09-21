---
title: edgeSearchEngine 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 787bbdc266baf130d6458e01e633b186368834da
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016322"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="1fc5a-103">edgeSearchEngine 资源类型</span><span class="sxs-lookup"><span data-stu-id="1fc5a-103">edgeSearchEngine resource type</span></span>

<span data-ttu-id="1fc5a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fc5a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1fc5a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1fc5a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1fc5a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1fc5a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fc5a-107">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="1fc5a-107">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="1fc5a-108">继承自 [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="1fc5a-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1fc5a-109">属性</span><span class="sxs-lookup"><span data-stu-id="1fc5a-109">Properties</span></span>
|<span data-ttu-id="1fc5a-110">属性</span><span class="sxs-lookup"><span data-stu-id="1fc5a-110">Property</span></span>|<span data-ttu-id="1fc5a-111">类型</span><span class="sxs-lookup"><span data-stu-id="1fc5a-111">Type</span></span>|<span data-ttu-id="1fc5a-112">说明</span><span class="sxs-lookup"><span data-stu-id="1fc5a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fc5a-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="1fc5a-113">edgeSearchEngineType</span></span>|[<span data-ttu-id="1fc5a-114">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="1fc5a-114">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="1fc5a-115">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="1fc5a-115">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="1fc5a-116">可取值为：`default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="1fc5a-116">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1fc5a-117">关系</span><span class="sxs-lookup"><span data-stu-id="1fc5a-117">Relationships</span></span>
<span data-ttu-id="1fc5a-118">无</span><span class="sxs-lookup"><span data-stu-id="1fc5a-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1fc5a-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1fc5a-119">JSON Representation</span></span>
<span data-ttu-id="1fc5a-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1fc5a-120">Here is a JSON representation of the resource.</span></span>
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






