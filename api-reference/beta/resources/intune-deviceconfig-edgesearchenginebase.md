---
title: edgeSearchEngineBase 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。 如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 30202e4be3c45f18dbcc3d010977baf97826a682
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392785"
---
# <a name="edgesearchenginebase-resource-type"></a><span data-ttu-id="701df-104">edgeSearchEngineBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="701df-104">edgeSearchEngineBase resource type</span></span>

> <span data-ttu-id="701df-105">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="701df-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="701df-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="701df-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="701df-107">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="701df-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="701df-108">允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="701df-108">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="701df-109">如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="701df-109">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>

## <a name="properties"></a><span data-ttu-id="701df-110">属性</span><span class="sxs-lookup"><span data-stu-id="701df-110">Properties</span></span>
|<span data-ttu-id="701df-111">属性</span><span class="sxs-lookup"><span data-stu-id="701df-111">Property</span></span>|<span data-ttu-id="701df-112">类型</span><span class="sxs-lookup"><span data-stu-id="701df-112">Type</span></span>|<span data-ttu-id="701df-113">说明</span><span class="sxs-lookup"><span data-stu-id="701df-113">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="701df-114">关系</span><span class="sxs-lookup"><span data-stu-id="701df-114">Relationships</span></span>
<span data-ttu-id="701df-115">无</span><span class="sxs-lookup"><span data-stu-id="701df-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="701df-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="701df-116">JSON Representation</span></span>
<span data-ttu-id="701df-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="701df-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngineBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineBase"
}
```




