---
title: windowsInformationProtectionIPRangeCollection 资源类型
description: Windows 信息保护 IP 范围集合
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 131694ba3ef67f1f87a1e40cd7545ad6e78717de
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468395"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="f7d6a-103">windowsInformationProtectionIPRangeCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="f7d6a-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

<span data-ttu-id="f7d6a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7d6a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7d6a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7d6a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7d6a-106">Windows 信息保护 IP 范围集合</span><span class="sxs-lookup"><span data-stu-id="f7d6a-106">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="f7d6a-107">属性</span><span class="sxs-lookup"><span data-stu-id="f7d6a-107">Properties</span></span>
|<span data-ttu-id="f7d6a-108">属性</span><span class="sxs-lookup"><span data-stu-id="f7d6a-108">Property</span></span>|<span data-ttu-id="f7d6a-109">类型</span><span class="sxs-lookup"><span data-stu-id="f7d6a-109">Type</span></span>|<span data-ttu-id="f7d6a-110">说明</span><span class="sxs-lookup"><span data-stu-id="f7d6a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7d6a-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f7d6a-111">displayName</span></span>|<span data-ttu-id="f7d6a-112">String</span><span class="sxs-lookup"><span data-stu-id="f7d6a-112">String</span></span>|<span data-ttu-id="f7d6a-113">显示名称</span><span class="sxs-lookup"><span data-stu-id="f7d6a-113">Display name</span></span>|
|<span data-ttu-id="f7d6a-114">ranges</span><span class="sxs-lookup"><span data-stu-id="f7d6a-114">ranges</span></span>|<span data-ttu-id="f7d6a-115">[ipRange](../resources/intune-mam-iprange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f7d6a-115">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="f7d6a-116">Internet 协议地址范围的集合</span><span class="sxs-lookup"><span data-stu-id="f7d6a-116">Collection of Internet protocol address ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7d6a-117">关系</span><span class="sxs-lookup"><span data-stu-id="f7d6a-117">Relationships</span></span>
<span data-ttu-id="f7d6a-118">无</span><span class="sxs-lookup"><span data-stu-id="f7d6a-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7d6a-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f7d6a-119">JSON Representation</span></span>
<span data-ttu-id="f7d6a-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7d6a-120">Here is a JSON representation of the resource.</span></span>
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







