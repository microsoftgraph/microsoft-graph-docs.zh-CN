---
title: edgeSearchEngine 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f39793a781a0660da4295bd0c4d69b5b8b305987
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465664"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="d05e1-103">edgeSearchEngine 资源类型</span><span class="sxs-lookup"><span data-stu-id="d05e1-103">edgeSearchEngine resource type</span></span>

<span data-ttu-id="d05e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d05e1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d05e1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d05e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d05e1-106">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="d05e1-106">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="d05e1-107">继承自 [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="d05e1-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d05e1-108">属性</span><span class="sxs-lookup"><span data-stu-id="d05e1-108">Properties</span></span>
|<span data-ttu-id="d05e1-109">属性</span><span class="sxs-lookup"><span data-stu-id="d05e1-109">Property</span></span>|<span data-ttu-id="d05e1-110">类型</span><span class="sxs-lookup"><span data-stu-id="d05e1-110">Type</span></span>|<span data-ttu-id="d05e1-111">说明</span><span class="sxs-lookup"><span data-stu-id="d05e1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d05e1-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="d05e1-112">edgeSearchEngineType</span></span>|[<span data-ttu-id="d05e1-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="d05e1-113">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="d05e1-114">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="d05e1-114">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="d05e1-115">可取值为：`default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="d05e1-115">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d05e1-116">关系</span><span class="sxs-lookup"><span data-stu-id="d05e1-116">Relationships</span></span>
<span data-ttu-id="d05e1-117">无</span><span class="sxs-lookup"><span data-stu-id="d05e1-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d05e1-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d05e1-118">JSON Representation</span></span>
<span data-ttu-id="d05e1-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d05e1-119">Here is a JSON representation of the resource.</span></span>
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







