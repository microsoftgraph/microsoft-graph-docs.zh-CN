---
title: edgeHomeButtonOpensCustomURL 资源类型
description: 显示 "主页" 按钮;单击 "主页" 按钮, 将加载特定的 URL。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2dad4baba5fd55b99efd6b2b7ebadf1973d6c9c8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551713"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="eb6b4-103">edgeHomeButtonOpensCustomURL 资源类型</span><span class="sxs-lookup"><span data-stu-id="eb6b4-103">edgeHomeButtonOpensCustomURL resource type</span></span>

> <span data-ttu-id="eb6b4-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eb6b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb6b4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eb6b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb6b4-106">显示 "主页" 按钮;单击 "主页" 按钮, 将加载特定的 URL。</span><span class="sxs-lookup"><span data-stu-id="eb6b4-106">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="eb6b4-107">继承自[edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eb6b4-107">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eb6b4-108">属性</span><span class="sxs-lookup"><span data-stu-id="eb6b4-108">Properties</span></span>
|<span data-ttu-id="eb6b4-109">属性</span><span class="sxs-lookup"><span data-stu-id="eb6b4-109">Property</span></span>|<span data-ttu-id="eb6b4-110">类型</span><span class="sxs-lookup"><span data-stu-id="eb6b4-110">Type</span></span>|<span data-ttu-id="eb6b4-111">说明</span><span class="sxs-lookup"><span data-stu-id="eb6b4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb6b4-112">homeButtonCustomURL</span><span class="sxs-lookup"><span data-stu-id="eb6b4-112">homeButtonCustomURL</span></span>|<span data-ttu-id="eb6b4-113">String</span><span class="sxs-lookup"><span data-stu-id="eb6b4-113">String</span></span>|<span data-ttu-id="eb6b4-114">要加载的特定 URL。</span><span class="sxs-lookup"><span data-stu-id="eb6b4-114">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb6b4-115">关系</span><span class="sxs-lookup"><span data-stu-id="eb6b4-115">Relationships</span></span>
<span data-ttu-id="eb6b4-116">无</span><span class="sxs-lookup"><span data-stu-id="eb6b4-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb6b4-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eb6b4-117">JSON Representation</span></span>
<span data-ttu-id="eb6b4-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb6b4-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeHomeButtonOpensCustomURL"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeHomeButtonOpensCustomURL",
  "homeButtonCustomURL": "String"
}
```





