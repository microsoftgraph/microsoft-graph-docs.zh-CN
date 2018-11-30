---
title: windowsInformationProtectionIPRangeCollection 资源类型
description: Windows 信息保护 IP 范围集合
ms.openlocfilehash: 41558014ec3d48af06788e15fc40786fe7f9aea4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008716"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="9d43d-103">windowsInformationProtectionIPRangeCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d43d-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="9d43d-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9d43d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d43d-105">Windows 信息保护 IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="9d43d-105">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="9d43d-106">属性</span><span class="sxs-lookup"><span data-stu-id="9d43d-106">Properties</span></span>
|<span data-ttu-id="9d43d-107">属性</span><span class="sxs-lookup"><span data-stu-id="9d43d-107">Property</span></span>|<span data-ttu-id="9d43d-108">类型</span><span class="sxs-lookup"><span data-stu-id="9d43d-108">Type</span></span>|<span data-ttu-id="9d43d-109">说明</span><span class="sxs-lookup"><span data-stu-id="9d43d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d43d-110">displayName</span><span class="sxs-lookup"><span data-stu-id="9d43d-110">displayName</span></span>|<span data-ttu-id="9d43d-111">String</span><span class="sxs-lookup"><span data-stu-id="9d43d-111">String</span></span>|<span data-ttu-id="9d43d-112">显示名称</span><span class="sxs-lookup"><span data-stu-id="9d43d-112">Display name</span></span>|
|<span data-ttu-id="9d43d-113">ranges</span><span class="sxs-lookup"><span data-stu-id="9d43d-113">ranges</span></span>|<span data-ttu-id="9d43d-114">[ipRange](../resources/intune-mam-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9d43d-114">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="9d43d-115">IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="9d43d-115">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d43d-116">关系</span><span class="sxs-lookup"><span data-stu-id="9d43d-116">Relationships</span></span>
<span data-ttu-id="9d43d-117">无</span><span class="sxs-lookup"><span data-stu-id="9d43d-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9d43d-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d43d-118">JSON Representation</span></span>
<span data-ttu-id="9d43d-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d43d-119">Here is a JSON representation of the resource.</span></span>
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



