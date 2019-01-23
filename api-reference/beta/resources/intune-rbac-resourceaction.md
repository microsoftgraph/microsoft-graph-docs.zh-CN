---
title: resourceAction 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5442ed8ee55005b1261da09d999e9c27053276d2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415262"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="5b64d-103">resourceAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b64d-103">resourceAction resource type</span></span>

> <span data-ttu-id="5b64d-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="5b64d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5b64d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5b64d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b64d-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5b64d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b64d-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5b64d-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="5b64d-108">属性</span><span class="sxs-lookup"><span data-stu-id="5b64d-108">Properties</span></span>
|<span data-ttu-id="5b64d-109">属性</span><span class="sxs-lookup"><span data-stu-id="5b64d-109">Property</span></span>|<span data-ttu-id="5b64d-110">类型</span><span class="sxs-lookup"><span data-stu-id="5b64d-110">Type</span></span>|<span data-ttu-id="5b64d-111">说明</span><span class="sxs-lookup"><span data-stu-id="5b64d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b64d-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="5b64d-112">allowedResourceActions</span></span>|<span data-ttu-id="5b64d-113">字符串集合</span><span class="sxs-lookup"><span data-stu-id="5b64d-113">String collection</span></span>|<span data-ttu-id="5b64d-114">允许的操作</span><span class="sxs-lookup"><span data-stu-id="5b64d-114">Allowed Actions</span></span>|
|<span data-ttu-id="5b64d-115">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="5b64d-115">notAllowedResourceActions</span></span>|<span data-ttu-id="5b64d-116">字符串集合</span><span class="sxs-lookup"><span data-stu-id="5b64d-116">String collection</span></span>|<span data-ttu-id="5b64d-117">不允许的操作</span><span class="sxs-lookup"><span data-stu-id="5b64d-117">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b64d-118">关系</span><span class="sxs-lookup"><span data-stu-id="5b64d-118">Relationships</span></span>
<span data-ttu-id="5b64d-119">无</span><span class="sxs-lookup"><span data-stu-id="5b64d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b64d-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5b64d-120">JSON Representation</span></span>
<span data-ttu-id="5b64d-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b64d-121">Here is a JSON representation of the resource.</span></span>
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




