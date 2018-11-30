---
title: windowsInformationProtectionResourceCollection 资源类型
description: Windows 信息保护资源集合
ms.openlocfilehash: c6840c8ebb272d0ad066556d9edab825b3fb50f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047987"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="c13a1-103">windowsInformationProtectionResourceCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="c13a1-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="c13a1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c13a1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c13a1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c13a1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c13a1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c13a1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c13a1-107">Windows 信息保护资源集合</span><span class="sxs-lookup"><span data-stu-id="c13a1-107">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="c13a1-108">属性</span><span class="sxs-lookup"><span data-stu-id="c13a1-108">Properties</span></span>
|<span data-ttu-id="c13a1-109">属性</span><span class="sxs-lookup"><span data-stu-id="c13a1-109">Property</span></span>|<span data-ttu-id="c13a1-110">类型</span><span class="sxs-lookup"><span data-stu-id="c13a1-110">Type</span></span>|<span data-ttu-id="c13a1-111">说明</span><span class="sxs-lookup"><span data-stu-id="c13a1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c13a1-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c13a1-112">displayName</span></span>|<span data-ttu-id="c13a1-113">String</span><span class="sxs-lookup"><span data-stu-id="c13a1-113">String</span></span>|<span data-ttu-id="c13a1-114">显示名称</span><span class="sxs-lookup"><span data-stu-id="c13a1-114">Display name</span></span>|
|<span data-ttu-id="c13a1-115">资源</span><span class="sxs-lookup"><span data-stu-id="c13a1-115">resources</span></span>|<span data-ttu-id="c13a1-116">字符串集合</span><span class="sxs-lookup"><span data-stu-id="c13a1-116">String collection</span></span>|<span data-ttu-id="c13a1-117">资源集合</span><span class="sxs-lookup"><span data-stu-id="c13a1-117">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="c13a1-118">关系</span><span class="sxs-lookup"><span data-stu-id="c13a1-118">Relationships</span></span>
<span data-ttu-id="c13a1-119">无</span><span class="sxs-lookup"><span data-stu-id="c13a1-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c13a1-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c13a1-120">JSON Representation</span></span>
<span data-ttu-id="c13a1-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c13a1-121">Here is a JSON representation of the resource.</span></span>
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





