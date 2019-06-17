---
title: resourceAction 资源类型
description: 资源的允许和不允许的操作的集合。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e49c06c8ca58f94948cc6458fd9dedd0adfa227e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993604"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="0956f-103">resourceAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="0956f-103">resourceAction resource type</span></span>

> <span data-ttu-id="0956f-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0956f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0956f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0956f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0956f-106">资源的允许和不允许的操作的集合。</span><span class="sxs-lookup"><span data-stu-id="0956f-106">Set of allowed and not allowed actions for a resource.</span></span>

## <a name="properties"></a><span data-ttu-id="0956f-107">属性</span><span class="sxs-lookup"><span data-stu-id="0956f-107">Properties</span></span>
|<span data-ttu-id="0956f-108">属性</span><span class="sxs-lookup"><span data-stu-id="0956f-108">Property</span></span>|<span data-ttu-id="0956f-109">类型</span><span class="sxs-lookup"><span data-stu-id="0956f-109">Type</span></span>|<span data-ttu-id="0956f-110">说明</span><span class="sxs-lookup"><span data-stu-id="0956f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0956f-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="0956f-111">allowedResourceActions</span></span>|<span data-ttu-id="0956f-112">字符串集合</span><span class="sxs-lookup"><span data-stu-id="0956f-112">String collection</span></span>|<span data-ttu-id="0956f-113">允许的操作</span><span class="sxs-lookup"><span data-stu-id="0956f-113">Allowed Actions</span></span>|
|<span data-ttu-id="0956f-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="0956f-114">notAllowedResourceActions</span></span>|<span data-ttu-id="0956f-115">字符串集合</span><span class="sxs-lookup"><span data-stu-id="0956f-115">String collection</span></span>|<span data-ttu-id="0956f-116">不允许操作。</span><span class="sxs-lookup"><span data-stu-id="0956f-116">Not Allowed Actions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0956f-117">关系</span><span class="sxs-lookup"><span data-stu-id="0956f-117">Relationships</span></span>
<span data-ttu-id="0956f-118">无</span><span class="sxs-lookup"><span data-stu-id="0956f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0956f-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0956f-119">JSON Representation</span></span>
<span data-ttu-id="0956f-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0956f-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```





