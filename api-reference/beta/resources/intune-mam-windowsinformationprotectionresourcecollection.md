---
title: windowsInformationProtectionResourceCollection 资源类型
description: Windows 信息保护资源集合
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c4a8ad51177507613c3fd84b524503d0e79c208f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424677"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="4bf11-103">windowsInformationProtectionResourceCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="4bf11-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="4bf11-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="4bf11-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4bf11-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4bf11-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4bf11-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4bf11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bf11-107">Windows 信息保护资源集合</span><span class="sxs-lookup"><span data-stu-id="4bf11-107">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="4bf11-108">属性</span><span class="sxs-lookup"><span data-stu-id="4bf11-108">Properties</span></span>
|<span data-ttu-id="4bf11-109">属性</span><span class="sxs-lookup"><span data-stu-id="4bf11-109">Property</span></span>|<span data-ttu-id="4bf11-110">类型</span><span class="sxs-lookup"><span data-stu-id="4bf11-110">Type</span></span>|<span data-ttu-id="4bf11-111">说明</span><span class="sxs-lookup"><span data-stu-id="4bf11-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bf11-112">displayName</span><span class="sxs-lookup"><span data-stu-id="4bf11-112">displayName</span></span>|<span data-ttu-id="4bf11-113">String</span><span class="sxs-lookup"><span data-stu-id="4bf11-113">String</span></span>|<span data-ttu-id="4bf11-114">显示名称</span><span class="sxs-lookup"><span data-stu-id="4bf11-114">Display name</span></span>|
|<span data-ttu-id="4bf11-115">资源</span><span class="sxs-lookup"><span data-stu-id="4bf11-115">resources</span></span>|<span data-ttu-id="4bf11-116">字符串集合</span><span class="sxs-lookup"><span data-stu-id="4bf11-116">String collection</span></span>|<span data-ttu-id="4bf11-117">资源集合</span><span class="sxs-lookup"><span data-stu-id="4bf11-117">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="4bf11-118">关系</span><span class="sxs-lookup"><span data-stu-id="4bf11-118">Relationships</span></span>
<span data-ttu-id="4bf11-119">无</span><span class="sxs-lookup"><span data-stu-id="4bf11-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4bf11-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4bf11-120">JSON Representation</span></span>
<span data-ttu-id="4bf11-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4bf11-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```




