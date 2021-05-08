---
title: educationOnPremisesInfo 资源类型
description: 用于将本地 Active Directory 用户帐户关联到其 Azure AD 用户对象的其他信息。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4c5da3180b1c15f2363bfd651d0f4e3d68f41b60
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232163"
---
# <a name="educationonpremisesinfo-resource-type"></a><span data-ttu-id="4c63b-103">educationOnPremisesInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="4c63b-103">educationOnPremisesInfo resource type</span></span>

<span data-ttu-id="4c63b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c63b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4c63b-105">用于将本地 Active Directory 用户帐户关联到其 Azure AD 用户对象的其他信息。</span><span class="sxs-lookup"><span data-stu-id="4c63b-105">Additional information used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span>

## <a name="properties"></a><span data-ttu-id="4c63b-106">属性</span><span class="sxs-lookup"><span data-stu-id="4c63b-106">Properties</span></span>

| <span data-ttu-id="4c63b-107">属性</span><span class="sxs-lookup"><span data-stu-id="4c63b-107">Property</span></span>    | <span data-ttu-id="4c63b-108">类型</span><span class="sxs-lookup"><span data-stu-id="4c63b-108">Type</span></span>   | <span data-ttu-id="4c63b-109">说明</span><span class="sxs-lookup"><span data-stu-id="4c63b-109">Description</span></span>                                                |
| :---------- | :----- | :--------------------------------------------------------- |
| <span data-ttu-id="4c63b-110">immutableId</span><span class="sxs-lookup"><span data-stu-id="4c63b-110">immutableId</span></span> | <span data-ttu-id="4c63b-111">String</span><span class="sxs-lookup"><span data-stu-id="4c63b-111">String</span></span> | <span data-ttu-id="4c63b-112">Active Directory 中用户对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4c63b-112">Unique identifier for the user object in Active Directory.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4c63b-113">关系</span><span class="sxs-lookup"><span data-stu-id="4c63b-113">Relationships</span></span>

<span data-ttu-id="4c63b-114">无。</span><span class="sxs-lookup"><span data-stu-id="4c63b-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c63b-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4c63b-115">JSON representation</span></span>

<span data-ttu-id="4c63b-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c63b-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationOnPremisesInfo"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationOnPremisesInfo",
  "immutableId": "String"
}
```
