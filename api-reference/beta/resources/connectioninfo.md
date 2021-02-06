---
title: connectionInfo 资源类型
description: connectionInfo 对象定义用于与资源通信的连接信息。
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 454dc7fcd045bb91819b39ad30f603191bab8380
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137714"
---
# <a name="connectioninfo-resource-type"></a><span data-ttu-id="e9451-103">connectionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="e9451-103">connectionInfo resource type</span></span>

<span data-ttu-id="e9451-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9451-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9451-105">connectionInfo 对象定义用于与 Azure AD 权利管理中的资源通信的资源定位器。</span><span class="sxs-lookup"><span data-stu-id="e9451-105">The connectionInfo object defines the resource locator that is used to communicate with a resource in Azure AD Entitlement Management.</span></span>

## <a name="properties"></a><span data-ttu-id="e9451-106">属性</span><span class="sxs-lookup"><span data-stu-id="e9451-106">Properties</span></span>
|<span data-ttu-id="e9451-107">属性</span><span class="sxs-lookup"><span data-stu-id="e9451-107">Property</span></span>|<span data-ttu-id="e9451-108">类型</span><span class="sxs-lookup"><span data-stu-id="e9451-108">Type</span></span>|<span data-ttu-id="e9451-109">说明</span><span class="sxs-lookup"><span data-stu-id="e9451-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9451-110">url</span><span class="sxs-lookup"><span data-stu-id="e9451-110">url</span></span>|<span data-ttu-id="e9451-111">String</span><span class="sxs-lookup"><span data-stu-id="e9451-111">String</span></span>|<span data-ttu-id="e9451-112">授权管理用于与访问包资源通信的终结点。</span><span class="sxs-lookup"><span data-stu-id="e9451-112">The endpoint that is used by Entitlement Management to communicate with the access package resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9451-113">关系</span><span class="sxs-lookup"><span data-stu-id="e9451-113">Relationships</span></span>
<span data-ttu-id="e9451-114">无。</span><span class="sxs-lookup"><span data-stu-id="e9451-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9451-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e9451-115">JSON representation</span></span>
<span data-ttu-id="e9451-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9451-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.connectionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.connectionInfo",
  "url": "String"
}
```
