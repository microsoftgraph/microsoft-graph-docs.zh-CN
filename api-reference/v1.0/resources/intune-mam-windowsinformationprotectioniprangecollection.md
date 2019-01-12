---
title: windowsInformationProtectionIPRangeCollection 资源类型
description: Windows 信息保护 IP 范围集合
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e9d23f8a6d771b116b35058c249866c70c7460d8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952655"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="dfb74-103">windowsInformationProtectionIPRangeCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="dfb74-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="dfb74-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="dfb74-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dfb74-105">Windows 信息保护 IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="dfb74-105">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="dfb74-106">属性</span><span class="sxs-lookup"><span data-stu-id="dfb74-106">Properties</span></span>
|<span data-ttu-id="dfb74-107">属性</span><span class="sxs-lookup"><span data-stu-id="dfb74-107">Property</span></span>|<span data-ttu-id="dfb74-108">类型</span><span class="sxs-lookup"><span data-stu-id="dfb74-108">Type</span></span>|<span data-ttu-id="dfb74-109">说明</span><span class="sxs-lookup"><span data-stu-id="dfb74-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfb74-110">displayName</span><span class="sxs-lookup"><span data-stu-id="dfb74-110">displayName</span></span>|<span data-ttu-id="dfb74-111">String</span><span class="sxs-lookup"><span data-stu-id="dfb74-111">String</span></span>|<span data-ttu-id="dfb74-112">显示名称</span><span class="sxs-lookup"><span data-stu-id="dfb74-112">Display name</span></span>|
|<span data-ttu-id="dfb74-113">ranges</span><span class="sxs-lookup"><span data-stu-id="dfb74-113">ranges</span></span>|<span data-ttu-id="dfb74-114">[ipRange](../resources/intune-mam-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dfb74-114">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="dfb74-115">IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="dfb74-115">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfb74-116">关系</span><span class="sxs-lookup"><span data-stu-id="dfb74-116">Relationships</span></span>
<span data-ttu-id="dfb74-117">无</span><span class="sxs-lookup"><span data-stu-id="dfb74-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dfb74-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dfb74-118">JSON Representation</span></span>
<span data-ttu-id="dfb74-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfb74-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionIPRangeCollection",
  "displayName": "String",
  "ranges": [
    {
      "@odata.type": "microsoft.graph.ipRange",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```



