---
title: edgeSearchEngine 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9828d2540f1b386302c18cde67811fe06fd9e50f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530048"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="7833f-103">edgeSearchEngine 资源类型</span><span class="sxs-lookup"><span data-stu-id="7833f-103">edgeSearchEngine resource type</span></span>

<span data-ttu-id="7833f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7833f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7833f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7833f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7833f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7833f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7833f-107">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="7833f-107">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="7833f-108">继承自 [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="7833f-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7833f-109">属性</span><span class="sxs-lookup"><span data-stu-id="7833f-109">Properties</span></span>
|<span data-ttu-id="7833f-110">属性</span><span class="sxs-lookup"><span data-stu-id="7833f-110">Property</span></span>|<span data-ttu-id="7833f-111">类型</span><span class="sxs-lookup"><span data-stu-id="7833f-111">Type</span></span>|<span data-ttu-id="7833f-112">说明</span><span class="sxs-lookup"><span data-stu-id="7833f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7833f-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="7833f-113">edgeSearchEngineType</span></span>|[<span data-ttu-id="7833f-114">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="7833f-114">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="7833f-115">允许 IT 管理员为 MDM 控制的设备设置预定义的默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="7833f-115">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="7833f-116">可取值为：`default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="7833f-116">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7833f-117">关系</span><span class="sxs-lookup"><span data-stu-id="7833f-117">Relationships</span></span>
<span data-ttu-id="7833f-118">无</span><span class="sxs-lookup"><span data-stu-id="7833f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7833f-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7833f-119">JSON Representation</span></span>
<span data-ttu-id="7833f-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7833f-120">Here is a JSON representation of the resource.</span></span>
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



