---
title: windowsInformationProtectionIPRangeCollection 资源类型
description: Windows 信息保护 IP 范围集合
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e57e8024365a3209f8d60d9558f76fed454a41a8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49207237"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="08712-103">windowsInformationProtectionIPRangeCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="08712-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

<span data-ttu-id="08712-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08712-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08712-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="08712-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08712-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="08712-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08712-107">Windows 信息保护 IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="08712-107">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="08712-108">属性</span><span class="sxs-lookup"><span data-stu-id="08712-108">Properties</span></span>
|<span data-ttu-id="08712-109">属性</span><span class="sxs-lookup"><span data-stu-id="08712-109">Property</span></span>|<span data-ttu-id="08712-110">类型</span><span class="sxs-lookup"><span data-stu-id="08712-110">Type</span></span>|<span data-ttu-id="08712-111">说明</span><span class="sxs-lookup"><span data-stu-id="08712-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08712-112">displayName</span><span class="sxs-lookup"><span data-stu-id="08712-112">displayName</span></span>|<span data-ttu-id="08712-113">String</span><span class="sxs-lookup"><span data-stu-id="08712-113">String</span></span>|<span data-ttu-id="08712-114">显示名称</span><span class="sxs-lookup"><span data-stu-id="08712-114">Display name</span></span>|
|<span data-ttu-id="08712-115">ranges</span><span class="sxs-lookup"><span data-stu-id="08712-115">ranges</span></span>|<span data-ttu-id="08712-116">[ipRange](../resources/intune-shared-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="08712-116">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="08712-117">IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="08712-117">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="08712-118">关系</span><span class="sxs-lookup"><span data-stu-id="08712-118">Relationships</span></span>
<span data-ttu-id="08712-119">无</span><span class="sxs-lookup"><span data-stu-id="08712-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08712-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="08712-120">JSON Representation</span></span>
<span data-ttu-id="08712-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08712-121">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.ipRange"
    }
  ]
}
```




