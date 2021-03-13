---
title: connectionInfo 资源类型
description: connectionInfo 对象定义用于与资源通信的连接信息。
author: hanki-microsoft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8bbab1e93cf5af0fcfbd401b6b726f3165f595b4
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761815"
---
# <a name="connectioninfo-resource-type"></a><span data-ttu-id="926d5-103">connectionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="926d5-103">connectionInfo resource type</span></span>

<span data-ttu-id="926d5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="926d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="926d5-105">connectionInfo 对象定义用于与 Azure AD 权利管理中的资源通信的资源定位器。</span><span class="sxs-lookup"><span data-stu-id="926d5-105">The connectionInfo object defines the resource locator that is used to communicate with a resource in Azure AD Entitlement Management.</span></span>

## <a name="properties"></a><span data-ttu-id="926d5-106">属性</span><span class="sxs-lookup"><span data-stu-id="926d5-106">Properties</span></span>
|<span data-ttu-id="926d5-107">属性</span><span class="sxs-lookup"><span data-stu-id="926d5-107">Property</span></span>|<span data-ttu-id="926d5-108">类型</span><span class="sxs-lookup"><span data-stu-id="926d5-108">Type</span></span>|<span data-ttu-id="926d5-109">说明</span><span class="sxs-lookup"><span data-stu-id="926d5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="926d5-110">url</span><span class="sxs-lookup"><span data-stu-id="926d5-110">url</span></span>|<span data-ttu-id="926d5-111">String</span><span class="sxs-lookup"><span data-stu-id="926d5-111">String</span></span>|<span data-ttu-id="926d5-112">授权管理用于与访问包资源通信的终结点。</span><span class="sxs-lookup"><span data-stu-id="926d5-112">The endpoint that is used by Entitlement Management to communicate with the access package resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="926d5-113">关系</span><span class="sxs-lookup"><span data-stu-id="926d5-113">Relationships</span></span>
<span data-ttu-id="926d5-114">无。</span><span class="sxs-lookup"><span data-stu-id="926d5-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="926d5-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="926d5-115">JSON representation</span></span>
<span data-ttu-id="926d5-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="926d5-116">The following is a JSON representation of the resource.</span></span>
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
