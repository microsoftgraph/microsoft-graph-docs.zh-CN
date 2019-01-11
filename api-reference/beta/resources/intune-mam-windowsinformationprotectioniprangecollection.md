---
title: windowsInformationProtectionIPRangeCollection 资源类型
description: Windows 信息保护 IP 范围集合
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 73995f6b8f5e376de53ec88772dc3713cc179f3a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838603"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="ae8ec-103">windowsInformationProtectionIPRangeCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="ae8ec-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="ae8ec-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ae8ec-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae8ec-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ae8ec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae8ec-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ae8ec-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ae8ec-107">Windows 信息保护 IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="ae8ec-107">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="ae8ec-108">属性</span><span class="sxs-lookup"><span data-stu-id="ae8ec-108">Properties</span></span>
|<span data-ttu-id="ae8ec-109">属性</span><span class="sxs-lookup"><span data-stu-id="ae8ec-109">Property</span></span>|<span data-ttu-id="ae8ec-110">类型</span><span class="sxs-lookup"><span data-stu-id="ae8ec-110">Type</span></span>|<span data-ttu-id="ae8ec-111">说明</span><span class="sxs-lookup"><span data-stu-id="ae8ec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae8ec-112">displayName</span><span class="sxs-lookup"><span data-stu-id="ae8ec-112">displayName</span></span>|<span data-ttu-id="ae8ec-113">String</span><span class="sxs-lookup"><span data-stu-id="ae8ec-113">String</span></span>|<span data-ttu-id="ae8ec-114">显示名称</span><span class="sxs-lookup"><span data-stu-id="ae8ec-114">Display name</span></span>|
|<span data-ttu-id="ae8ec-115">ranges</span><span class="sxs-lookup"><span data-stu-id="ae8ec-115">ranges</span></span>|<span data-ttu-id="ae8ec-116">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ae8ec-116">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="ae8ec-117">IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="ae8ec-117">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae8ec-118">关系</span><span class="sxs-lookup"><span data-stu-id="ae8ec-118">Relationships</span></span>
<span data-ttu-id="ae8ec-119">无</span><span class="sxs-lookup"><span data-stu-id="ae8ec-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ae8ec-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ae8ec-120">JSON Representation</span></span>
<span data-ttu-id="ae8ec-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae8ec-121">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```





