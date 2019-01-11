---
title: windowsInformationProtectionIPRangeCollection 资源类型
description: Windows 信息保护 IP 范围集合
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2ba01b8a4385b5c06cc1e6a95441e9b7946a116d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839744"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="caf5b-103">windowsInformationProtectionIPRangeCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="caf5b-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="caf5b-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="caf5b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="caf5b-105">Windows 信息保护 IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="caf5b-105">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="caf5b-106">属性</span><span class="sxs-lookup"><span data-stu-id="caf5b-106">Properties</span></span>
|<span data-ttu-id="caf5b-107">属性</span><span class="sxs-lookup"><span data-stu-id="caf5b-107">Property</span></span>|<span data-ttu-id="caf5b-108">类型</span><span class="sxs-lookup"><span data-stu-id="caf5b-108">Type</span></span>|<span data-ttu-id="caf5b-109">说明</span><span class="sxs-lookup"><span data-stu-id="caf5b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caf5b-110">displayName</span><span class="sxs-lookup"><span data-stu-id="caf5b-110">displayName</span></span>|<span data-ttu-id="caf5b-111">String</span><span class="sxs-lookup"><span data-stu-id="caf5b-111">String</span></span>|<span data-ttu-id="caf5b-112">显示名称</span><span class="sxs-lookup"><span data-stu-id="caf5b-112">Display name</span></span>|
|<span data-ttu-id="caf5b-113">ranges</span><span class="sxs-lookup"><span data-stu-id="caf5b-113">ranges</span></span>|<span data-ttu-id="caf5b-114">[ipRange](../resources/intune-mam-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="caf5b-114">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="caf5b-115">IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="caf5b-115">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="caf5b-116">关系</span><span class="sxs-lookup"><span data-stu-id="caf5b-116">Relationships</span></span>
<span data-ttu-id="caf5b-117">无</span><span class="sxs-lookup"><span data-stu-id="caf5b-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="caf5b-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="caf5b-118">JSON Representation</span></span>
<span data-ttu-id="caf5b-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="caf5b-119">Here is a JSON representation of the resource.</span></span>
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



