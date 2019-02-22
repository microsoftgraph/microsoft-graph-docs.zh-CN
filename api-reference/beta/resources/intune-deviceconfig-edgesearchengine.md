---
title: edgeSearchEngine 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 75c5864a9f9d78b9ea9555c31ae1bc2baec28e49
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163215"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="c7068-103">edgeSearchEngine 资源类型</span><span class="sxs-lookup"><span data-stu-id="c7068-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="c7068-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c7068-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7068-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c7068-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7068-106">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="c7068-106">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="c7068-107">继承自 [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="c7068-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c7068-108">属性</span><span class="sxs-lookup"><span data-stu-id="c7068-108">Properties</span></span>
|<span data-ttu-id="c7068-109">属性</span><span class="sxs-lookup"><span data-stu-id="c7068-109">Property</span></span>|<span data-ttu-id="c7068-110">类型</span><span class="sxs-lookup"><span data-stu-id="c7068-110">Type</span></span>|<span data-ttu-id="c7068-111">说明</span><span class="sxs-lookup"><span data-stu-id="c7068-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7068-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="c7068-112">edgeSearchEngineType</span></span>|[<span data-ttu-id="c7068-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="c7068-113">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="c7068-114">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="c7068-114">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="c7068-115">可取值为：`default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="c7068-115">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7068-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="c7068-116">Relationships</span></span>
<span data-ttu-id="c7068-117">无</span><span class="sxs-lookup"><span data-stu-id="c7068-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7068-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7068-118">JSON Representation</span></span>
<span data-ttu-id="c7068-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7068-119">Here is a JSON representation of the resource.</span></span>
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




