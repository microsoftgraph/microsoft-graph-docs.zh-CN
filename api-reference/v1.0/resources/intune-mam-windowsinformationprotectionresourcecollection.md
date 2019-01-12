---
title: windowsInformationProtectionResourceCollection 资源类型
description: Windows 信息保护资源集合
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a913f90c2fed24a524e07b8dca1b629ebd9795f6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981215"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="10825-103">windowsInformationProtectionResourceCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="10825-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="10825-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="10825-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10825-105">Windows 信息保护资源集合</span><span class="sxs-lookup"><span data-stu-id="10825-105">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="10825-106">属性</span><span class="sxs-lookup"><span data-stu-id="10825-106">Properties</span></span>
|<span data-ttu-id="10825-107">属性</span><span class="sxs-lookup"><span data-stu-id="10825-107">Property</span></span>|<span data-ttu-id="10825-108">类型</span><span class="sxs-lookup"><span data-stu-id="10825-108">Type</span></span>|<span data-ttu-id="10825-109">说明</span><span class="sxs-lookup"><span data-stu-id="10825-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10825-110">displayName</span><span class="sxs-lookup"><span data-stu-id="10825-110">displayName</span></span>|<span data-ttu-id="10825-111">String</span><span class="sxs-lookup"><span data-stu-id="10825-111">String</span></span>|<span data-ttu-id="10825-112">显示名称</span><span class="sxs-lookup"><span data-stu-id="10825-112">Display name</span></span>|
|<span data-ttu-id="10825-113">资源</span><span class="sxs-lookup"><span data-stu-id="10825-113">resources</span></span>|<span data-ttu-id="10825-114">字符串集合</span><span class="sxs-lookup"><span data-stu-id="10825-114">String collection</span></span>|<span data-ttu-id="10825-115">资源集合</span><span class="sxs-lookup"><span data-stu-id="10825-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="10825-116">关系</span><span class="sxs-lookup"><span data-stu-id="10825-116">Relationships</span></span>
<span data-ttu-id="10825-117">无</span><span class="sxs-lookup"><span data-stu-id="10825-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="10825-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10825-118">JSON Representation</span></span>
<span data-ttu-id="10825-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10825-119">Here is a JSON representation of the resource.</span></span>
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



