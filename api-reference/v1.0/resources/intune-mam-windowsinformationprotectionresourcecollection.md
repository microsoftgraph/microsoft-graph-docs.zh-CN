---
title: windowsInformationProtectionResourceCollection 资源类型
description: Windows 信息保护资源集合
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0df0ebc3c67e7cf9bc18240f75d620442f80e0d6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844350"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="2c11e-103">windowsInformationProtectionResourceCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="2c11e-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="2c11e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2c11e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2c11e-105">Windows 信息保护资源集合</span><span class="sxs-lookup"><span data-stu-id="2c11e-105">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="2c11e-106">属性</span><span class="sxs-lookup"><span data-stu-id="2c11e-106">Properties</span></span>
|<span data-ttu-id="2c11e-107">属性</span><span class="sxs-lookup"><span data-stu-id="2c11e-107">Property</span></span>|<span data-ttu-id="2c11e-108">类型</span><span class="sxs-lookup"><span data-stu-id="2c11e-108">Type</span></span>|<span data-ttu-id="2c11e-109">说明</span><span class="sxs-lookup"><span data-stu-id="2c11e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c11e-110">displayName</span><span class="sxs-lookup"><span data-stu-id="2c11e-110">displayName</span></span>|<span data-ttu-id="2c11e-111">String</span><span class="sxs-lookup"><span data-stu-id="2c11e-111">String</span></span>|<span data-ttu-id="2c11e-112">显示名称</span><span class="sxs-lookup"><span data-stu-id="2c11e-112">Display name</span></span>|
|<span data-ttu-id="2c11e-113">资源</span><span class="sxs-lookup"><span data-stu-id="2c11e-113">resources</span></span>|<span data-ttu-id="2c11e-114">字符串集合</span><span class="sxs-lookup"><span data-stu-id="2c11e-114">String collection</span></span>|<span data-ttu-id="2c11e-115">资源集合</span><span class="sxs-lookup"><span data-stu-id="2c11e-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c11e-116">关系</span><span class="sxs-lookup"><span data-stu-id="2c11e-116">Relationships</span></span>
<span data-ttu-id="2c11e-117">无</span><span class="sxs-lookup"><span data-stu-id="2c11e-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2c11e-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2c11e-118">JSON Representation</span></span>
<span data-ttu-id="2c11e-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c11e-119">Here is a JSON representation of the resource.</span></span>
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



