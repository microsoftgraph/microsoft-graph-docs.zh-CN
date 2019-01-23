---
title: edgeSearchEngine 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b868be9ff34e85516e34040cb3ccb6f0efb95cb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402368"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="9f0fb-103">edgeSearchEngine 资源类型</span><span class="sxs-lookup"><span data-stu-id="9f0fb-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="9f0fb-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="9f0fb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9f0fb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9f0fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f0fb-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9f0fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f0fb-107">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="9f0fb-107">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="9f0fb-108">继承自 [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="9f0fb-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9f0fb-109">属性</span><span class="sxs-lookup"><span data-stu-id="9f0fb-109">Properties</span></span>
|<span data-ttu-id="9f0fb-110">属性</span><span class="sxs-lookup"><span data-stu-id="9f0fb-110">Property</span></span>|<span data-ttu-id="9f0fb-111">类型</span><span class="sxs-lookup"><span data-stu-id="9f0fb-111">Type</span></span>|<span data-ttu-id="9f0fb-112">说明</span><span class="sxs-lookup"><span data-stu-id="9f0fb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f0fb-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="9f0fb-113">edgeSearchEngineType</span></span>|[<span data-ttu-id="9f0fb-114">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="9f0fb-114">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="9f0fb-115">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="9f0fb-115">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="9f0fb-116">可取值为：`default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="9f0fb-116">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f0fb-117">Relationships</span><span class="sxs-lookup"><span data-stu-id="9f0fb-117">Relationships</span></span>
<span data-ttu-id="9f0fb-118">无</span><span class="sxs-lookup"><span data-stu-id="9f0fb-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f0fb-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9f0fb-119">JSON Representation</span></span>
<span data-ttu-id="9f0fb-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f0fb-120">Here is a JSON representation of the resource.</span></span>
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




