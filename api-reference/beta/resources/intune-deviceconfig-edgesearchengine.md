---
title: edgeSearchEngine 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b59fa163fe453d4f26dd71afa24edf9ac37d9d41
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953236"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="bd5e5-103">edgeSearchEngine 资源类型</span><span class="sxs-lookup"><span data-stu-id="bd5e5-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="bd5e5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bd5e5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd5e5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bd5e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd5e5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bd5e5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd5e5-107">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="bd5e5-107">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="bd5e5-108">继承自 [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="bd5e5-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bd5e5-109">属性</span><span class="sxs-lookup"><span data-stu-id="bd5e5-109">Properties</span></span>
|<span data-ttu-id="bd5e5-110">属性</span><span class="sxs-lookup"><span data-stu-id="bd5e5-110">Property</span></span>|<span data-ttu-id="bd5e5-111">类型</span><span class="sxs-lookup"><span data-stu-id="bd5e5-111">Type</span></span>|<span data-ttu-id="bd5e5-112">说明</span><span class="sxs-lookup"><span data-stu-id="bd5e5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd5e5-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="bd5e5-113">edgeSearchEngineType</span></span>|[<span data-ttu-id="bd5e5-114">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="bd5e5-114">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="bd5e5-115">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="bd5e5-115">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="bd5e5-116">可取值为：`default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="bd5e5-116">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd5e5-117">Relationships</span><span class="sxs-lookup"><span data-stu-id="bd5e5-117">Relationships</span></span>
<span data-ttu-id="bd5e5-118">无</span><span class="sxs-lookup"><span data-stu-id="bd5e5-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bd5e5-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bd5e5-119">JSON Representation</span></span>
<span data-ttu-id="bd5e5-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd5e5-120">Here is a JSON representation of the resource.</span></span>
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





