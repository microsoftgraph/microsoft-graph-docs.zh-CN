---
title: windowsInformationProtectionResourceCollection 资源类型
description: Windows 信息保护资源集合
author: tfitzmac
ms.openlocfilehash: 8e037ff53e11566aee7d79d2c3bbe5b1075b83a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327830"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="75d96-103">windowsInformationProtectionResourceCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="75d96-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="75d96-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="75d96-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="75d96-105">Windows 信息保护资源集合</span><span class="sxs-lookup"><span data-stu-id="75d96-105">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="75d96-106">属性</span><span class="sxs-lookup"><span data-stu-id="75d96-106">Properties</span></span>
|<span data-ttu-id="75d96-107">属性</span><span class="sxs-lookup"><span data-stu-id="75d96-107">Property</span></span>|<span data-ttu-id="75d96-108">类型</span><span class="sxs-lookup"><span data-stu-id="75d96-108">Type</span></span>|<span data-ttu-id="75d96-109">说明</span><span class="sxs-lookup"><span data-stu-id="75d96-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75d96-110">displayName</span><span class="sxs-lookup"><span data-stu-id="75d96-110">displayName</span></span>|<span data-ttu-id="75d96-111">String</span><span class="sxs-lookup"><span data-stu-id="75d96-111">String</span></span>|<span data-ttu-id="75d96-112">显示名称</span><span class="sxs-lookup"><span data-stu-id="75d96-112">Display name</span></span>|
|<span data-ttu-id="75d96-113">资源</span><span class="sxs-lookup"><span data-stu-id="75d96-113">resources</span></span>|<span data-ttu-id="75d96-114">字符串集合</span><span class="sxs-lookup"><span data-stu-id="75d96-114">String collection</span></span>|<span data-ttu-id="75d96-115">资源集合</span><span class="sxs-lookup"><span data-stu-id="75d96-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="75d96-116">关系</span><span class="sxs-lookup"><span data-stu-id="75d96-116">Relationships</span></span>
<span data-ttu-id="75d96-117">无</span><span class="sxs-lookup"><span data-stu-id="75d96-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="75d96-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="75d96-118">JSON Representation</span></span>
<span data-ttu-id="75d96-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75d96-119">Here is a JSON representation of the resource.</span></span>
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



