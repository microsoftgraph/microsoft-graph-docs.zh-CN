---
title: edgeSearchEngine 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1be131396c67f5af37a10ab3e0b7b1248cc8c4bf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532543"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="dd199-103">edgeSearchEngine 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd199-103">edgeSearchEngine resource type</span></span>

<span data-ttu-id="dd199-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd199-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd199-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dd199-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd199-106">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="dd199-106">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="dd199-107">继承自 [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="dd199-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dd199-108">属性</span><span class="sxs-lookup"><span data-stu-id="dd199-108">Properties</span></span>
|<span data-ttu-id="dd199-109">属性</span><span class="sxs-lookup"><span data-stu-id="dd199-109">Property</span></span>|<span data-ttu-id="dd199-110">类型</span><span class="sxs-lookup"><span data-stu-id="dd199-110">Type</span></span>|<span data-ttu-id="dd199-111">说明</span><span class="sxs-lookup"><span data-stu-id="dd199-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd199-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="dd199-112">edgeSearchEngineType</span></span>|[<span data-ttu-id="dd199-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="dd199-113">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="dd199-114">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="dd199-114">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="dd199-115">可取值为：`default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="dd199-115">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd199-116">关系</span><span class="sxs-lookup"><span data-stu-id="dd199-116">Relationships</span></span>
<span data-ttu-id="dd199-117">无</span><span class="sxs-lookup"><span data-stu-id="dd199-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd199-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd199-118">JSON Representation</span></span>
<span data-ttu-id="dd199-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd199-119">Here is a JSON representation of the resource.</span></span>
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




