---
title: edgeSearchEngine 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7a58cbed251773559beb2589893ab9759d4758fa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819906"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="a4fdc-103">edgeSearchEngine 资源类型</span><span class="sxs-lookup"><span data-stu-id="a4fdc-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="a4fdc-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a4fdc-105">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-105">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="a4fdc-106">继承自 [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="a4fdc-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a4fdc-107">属性</span><span class="sxs-lookup"><span data-stu-id="a4fdc-107">Properties</span></span>
|<span data-ttu-id="a4fdc-108">属性</span><span class="sxs-lookup"><span data-stu-id="a4fdc-108">Property</span></span>|<span data-ttu-id="a4fdc-109">类型</span><span class="sxs-lookup"><span data-stu-id="a4fdc-109">Type</span></span>|<span data-ttu-id="a4fdc-110">说明</span><span class="sxs-lookup"><span data-stu-id="a4fdc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4fdc-111">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="a4fdc-111">edgeSearchEngineType</span></span>|[<span data-ttu-id="a4fdc-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="a4fdc-112">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="a4fdc-113">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-113">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="a4fdc-114">可取值为：`default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-114">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4fdc-115">Relationships</span><span class="sxs-lookup"><span data-stu-id="a4fdc-115">Relationships</span></span>
<span data-ttu-id="a4fdc-116">无</span><span class="sxs-lookup"><span data-stu-id="a4fdc-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a4fdc-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a4fdc-117">JSON Representation</span></span>
<span data-ttu-id="a4fdc-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-118">Here is a JSON representation of the resource.</span></span>
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



