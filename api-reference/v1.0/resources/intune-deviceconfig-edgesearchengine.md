---
title: edgeSearchEngine 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 040ff093004cdb1d31dde748a7ad26f03ce08b10
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056791"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="cdad3-103">edgeSearchEngine 资源类型</span><span class="sxs-lookup"><span data-stu-id="cdad3-103">edgeSearchEngine resource type</span></span>

<span data-ttu-id="cdad3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdad3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cdad3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cdad3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdad3-106">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="cdad3-106">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="cdad3-107">继承自 [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="cdad3-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cdad3-108">属性</span><span class="sxs-lookup"><span data-stu-id="cdad3-108">Properties</span></span>
|<span data-ttu-id="cdad3-109">属性</span><span class="sxs-lookup"><span data-stu-id="cdad3-109">Property</span></span>|<span data-ttu-id="cdad3-110">类型</span><span class="sxs-lookup"><span data-stu-id="cdad3-110">Type</span></span>|<span data-ttu-id="cdad3-111">说明</span><span class="sxs-lookup"><span data-stu-id="cdad3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdad3-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="cdad3-112">edgeSearchEngineType</span></span>|[<span data-ttu-id="cdad3-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="cdad3-113">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="cdad3-114">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="cdad3-114">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="cdad3-115">可取值为：`default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="cdad3-115">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cdad3-116">关系</span><span class="sxs-lookup"><span data-stu-id="cdad3-116">Relationships</span></span>
<span data-ttu-id="cdad3-117">无</span><span class="sxs-lookup"><span data-stu-id="cdad3-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cdad3-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cdad3-118">JSON Representation</span></span>
<span data-ttu-id="cdad3-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cdad3-119">Here is a JSON representation of the resource.</span></span>
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









