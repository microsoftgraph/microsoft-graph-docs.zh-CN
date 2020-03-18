---
title: edgeSearchEngine 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9471c92dc88d49426a7f8c41f73708594b7cbf8c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791861"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="f8b9a-103">edgeSearchEngine 资源类型</span><span class="sxs-lookup"><span data-stu-id="f8b9a-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="f8b9a-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f8b9a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8b9a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f8b9a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8b9a-106">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="f8b9a-106">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="f8b9a-107">继承自 [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="f8b9a-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f8b9a-108">属性</span><span class="sxs-lookup"><span data-stu-id="f8b9a-108">Properties</span></span>
|<span data-ttu-id="f8b9a-109">属性</span><span class="sxs-lookup"><span data-stu-id="f8b9a-109">Property</span></span>|<span data-ttu-id="f8b9a-110">类型</span><span class="sxs-lookup"><span data-stu-id="f8b9a-110">Type</span></span>|<span data-ttu-id="f8b9a-111">说明</span><span class="sxs-lookup"><span data-stu-id="f8b9a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8b9a-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="f8b9a-112">edgeSearchEngineType</span></span>|[<span data-ttu-id="f8b9a-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="f8b9a-113">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="f8b9a-114">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="f8b9a-114">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="f8b9a-115">可取值为：`default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="f8b9a-115">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8b9a-116">关系</span><span class="sxs-lookup"><span data-stu-id="f8b9a-116">Relationships</span></span>
<span data-ttu-id="f8b9a-117">无</span><span class="sxs-lookup"><span data-stu-id="f8b9a-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8b9a-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f8b9a-118">JSON Representation</span></span>
<span data-ttu-id="f8b9a-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8b9a-119">Here is a JSON representation of the resource.</span></span>
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



