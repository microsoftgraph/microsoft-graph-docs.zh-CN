---
title: edgeSearchEngine 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b5ea2d73724400c033a3bd8e1148e04af8d390be
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755068"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="8fddf-103">edgeSearchEngine 资源类型</span><span class="sxs-lookup"><span data-stu-id="8fddf-103">edgeSearchEngine resource type</span></span>

<span data-ttu-id="8fddf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fddf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8fddf-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8fddf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fddf-106">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="8fddf-106">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="8fddf-107">继承自 [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="8fddf-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8fddf-108">属性</span><span class="sxs-lookup"><span data-stu-id="8fddf-108">Properties</span></span>
|<span data-ttu-id="8fddf-109">属性</span><span class="sxs-lookup"><span data-stu-id="8fddf-109">Property</span></span>|<span data-ttu-id="8fddf-110">类型</span><span class="sxs-lookup"><span data-stu-id="8fddf-110">Type</span></span>|<span data-ttu-id="8fddf-111">Description</span><span class="sxs-lookup"><span data-stu-id="8fddf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fddf-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="8fddf-112">edgeSearchEngineType</span></span>|[<span data-ttu-id="8fddf-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="8fddf-113">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="8fddf-114">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="8fddf-114">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="8fddf-115">可取值为：`default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="8fddf-115">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fddf-116">关系</span><span class="sxs-lookup"><span data-stu-id="8fddf-116">Relationships</span></span>
<span data-ttu-id="8fddf-117">无</span><span class="sxs-lookup"><span data-stu-id="8fddf-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8fddf-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8fddf-118">JSON Representation</span></span>
<span data-ttu-id="8fddf-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8fddf-119">Here is a JSON representation of the resource.</span></span>
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




