---
title: edgeSearchEngineBase 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。 如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 00d9858eb8277b804d5fb90acd8efc9174c7c8bc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161969"
---
# <a name="edgesearchenginebase-resource-type"></a><span data-ttu-id="a4f52-104">edgeSearchEngineBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="a4f52-104">edgeSearchEngineBase resource type</span></span>

> <span data-ttu-id="a4f52-105">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a4f52-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4f52-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a4f52-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4f52-107">允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="a4f52-107">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="a4f52-108">如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="a4f52-108">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>

## <a name="properties"></a><span data-ttu-id="a4f52-109">属性</span><span class="sxs-lookup"><span data-stu-id="a4f52-109">Properties</span></span>
|<span data-ttu-id="a4f52-110">属性</span><span class="sxs-lookup"><span data-stu-id="a4f52-110">Property</span></span>|<span data-ttu-id="a4f52-111">类型</span><span class="sxs-lookup"><span data-stu-id="a4f52-111">Type</span></span>|<span data-ttu-id="a4f52-112">说明</span><span class="sxs-lookup"><span data-stu-id="a4f52-112">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="a4f52-113">关系</span><span class="sxs-lookup"><span data-stu-id="a4f52-113">Relationships</span></span>
<span data-ttu-id="a4f52-114">无</span><span class="sxs-lookup"><span data-stu-id="a4f52-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4f52-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a4f52-115">JSON Representation</span></span>
<span data-ttu-id="a4f52-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4f52-116">Here is a JSON representation of the resource.</span></span>
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




