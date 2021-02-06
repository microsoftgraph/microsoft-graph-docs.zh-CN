---
title: userRegistrationMethodCount 资源类型
description: 为身份验证方法注册的用户数。
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 8e4c19c48771ccd0bd1dd1f1a4b049334266834a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132930"
---
# <a name="userregistrationmethodcount-resource-type"></a><span data-ttu-id="7073f-103">userRegistrationMethodCount 资源类型</span><span class="sxs-lookup"><span data-stu-id="7073f-103">userRegistrationMethodCount resource type</span></span>

<span data-ttu-id="7073f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7073f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7073f-105">为身份验证方法注册的用户数。</span><span class="sxs-lookup"><span data-stu-id="7073f-105">Number of users registered for an authentication method.</span></span>

## <a name="properties"></a><span data-ttu-id="7073f-106">属性</span><span class="sxs-lookup"><span data-stu-id="7073f-106">Properties</span></span>
|<span data-ttu-id="7073f-107">属性</span><span class="sxs-lookup"><span data-stu-id="7073f-107">Property</span></span>|<span data-ttu-id="7073f-108">类型</span><span class="sxs-lookup"><span data-stu-id="7073f-108">Type</span></span>|<span data-ttu-id="7073f-109">说明</span><span class="sxs-lookup"><span data-stu-id="7073f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7073f-110">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7073f-110">authenticationMethod</span></span>|<span data-ttu-id="7073f-111">字符串</span><span class="sxs-lookup"><span data-stu-id="7073f-111">String</span></span>|<span data-ttu-id="7073f-112">身份验证方法的名称。</span><span class="sxs-lookup"><span data-stu-id="7073f-112">Name of authentication method.</span></span>|
|<span data-ttu-id="7073f-113">userCount</span><span class="sxs-lookup"><span data-stu-id="7073f-113">userCount</span></span>|<span data-ttu-id="7073f-114">Int64</span><span class="sxs-lookup"><span data-stu-id="7073f-114">Int64</span></span>|<span data-ttu-id="7073f-115">注册的用户数。</span><span class="sxs-lookup"><span data-stu-id="7073f-115">Number of users registered.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7073f-116">关系</span><span class="sxs-lookup"><span data-stu-id="7073f-116">Relationships</span></span>
<span data-ttu-id="7073f-117">无。</span><span class="sxs-lookup"><span data-stu-id="7073f-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7073f-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7073f-118">JSON representation</span></span>
<span data-ttu-id="7073f-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7073f-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationMethodCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationMethodCount",
  "authenticationMethod": "String",
  "userCount": "Integer"
}
```
