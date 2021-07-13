---
title: tenantContactInformation 资源类型
description: 表示托管租户的联系人。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: b60005cf60a9ac1b96a3b650a853f8b198d27e48
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402394"
---
# <a name="tenantcontactinformation-resource-type"></a><span data-ttu-id="94d73-103">tenantContactInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="94d73-103">tenantContactInformation resource type</span></span>

<span data-ttu-id="94d73-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="94d73-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94d73-105">表示托管租户的联系人。</span><span class="sxs-lookup"><span data-stu-id="94d73-105">Represents a contact at a managed tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="94d73-106">属性</span><span class="sxs-lookup"><span data-stu-id="94d73-106">Properties</span></span>
|<span data-ttu-id="94d73-107">属性</span><span class="sxs-lookup"><span data-stu-id="94d73-107">Property</span></span>|<span data-ttu-id="94d73-108">类型</span><span class="sxs-lookup"><span data-stu-id="94d73-108">Type</span></span>|<span data-ttu-id="94d73-109">说明</span><span class="sxs-lookup"><span data-stu-id="94d73-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94d73-110">email</span><span class="sxs-lookup"><span data-stu-id="94d73-110">email</span></span>|<span data-ttu-id="94d73-111">String</span><span class="sxs-lookup"><span data-stu-id="94d73-111">String</span></span>|<span data-ttu-id="94d73-112">联系人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="94d73-112">The email address for the contact.</span></span> <span data-ttu-id="94d73-113">可选</span><span class="sxs-lookup"><span data-stu-id="94d73-113">Optional</span></span>|
|<span data-ttu-id="94d73-114">name</span><span class="sxs-lookup"><span data-stu-id="94d73-114">name</span></span>|<span data-ttu-id="94d73-115">String</span><span class="sxs-lookup"><span data-stu-id="94d73-115">String</span></span>|<span data-ttu-id="94d73-116">联系人的名称。</span><span class="sxs-lookup"><span data-stu-id="94d73-116">The name for the contact.</span></span> <span data-ttu-id="94d73-117">必填。</span><span class="sxs-lookup"><span data-stu-id="94d73-117">Required.</span></span>|
|<span data-ttu-id="94d73-118">notes</span><span class="sxs-lookup"><span data-stu-id="94d73-118">notes</span></span>|<span data-ttu-id="94d73-119">String</span><span class="sxs-lookup"><span data-stu-id="94d73-119">String</span></span>|<span data-ttu-id="94d73-120">与联系人关联的注释。</span><span class="sxs-lookup"><span data-stu-id="94d73-120">The notes associated with the contact.</span></span> <span data-ttu-id="94d73-121">可选</span><span class="sxs-lookup"><span data-stu-id="94d73-121">Optional</span></span>|
|<span data-ttu-id="94d73-122">phone</span><span class="sxs-lookup"><span data-stu-id="94d73-122">phone</span></span>|<span data-ttu-id="94d73-123">String</span><span class="sxs-lookup"><span data-stu-id="94d73-123">String</span></span>|<span data-ttu-id="94d73-124">联系人的电话号码。</span><span class="sxs-lookup"><span data-stu-id="94d73-124">The phone number for the contact.</span></span> <span data-ttu-id="94d73-125">可选。</span><span class="sxs-lookup"><span data-stu-id="94d73-125">Optional.</span></span>|
|<span data-ttu-id="94d73-126">title</span><span class="sxs-lookup"><span data-stu-id="94d73-126">title</span></span>|<span data-ttu-id="94d73-127">String</span><span class="sxs-lookup"><span data-stu-id="94d73-127">String</span></span>|<span data-ttu-id="94d73-128">联系人的标题。</span><span class="sxs-lookup"><span data-stu-id="94d73-128">The title for the contact.</span></span> <span data-ttu-id="94d73-129">必填。</span><span class="sxs-lookup"><span data-stu-id="94d73-129">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94d73-130">关系</span><span class="sxs-lookup"><span data-stu-id="94d73-130">Relationships</span></span>
<span data-ttu-id="94d73-131">无。</span><span class="sxs-lookup"><span data-stu-id="94d73-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="94d73-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94d73-132">JSON representation</span></span>
<span data-ttu-id="94d73-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94d73-133">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.tenantContactInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantContactInformation",
  "name": "String",
  "title": "String",
  "email": "String",
  "phone": "String",
  "notes": "String"
}
```
