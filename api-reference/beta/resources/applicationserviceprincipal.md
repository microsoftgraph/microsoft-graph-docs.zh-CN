---
title: applicationServicePrincipal 资源类型
description: 应用程序和 servicePrincipal 的组合。
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c3a6d0d1017f89587f1f826c4225eefc51dc5edb
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2019
ms.locfileid: "35147898"
---
# <a name="applicationserviceprincipal-resource-type"></a><span data-ttu-id="1c628-103">applicationServicePrincipal 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c628-103">applicationServicePrincipal resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c628-104">当添加了 Azure AD 应用程序库中的应用程序实例时, 将在目录中创建[application](../resources/application.md)和[servicePrincipal](../resources/serviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1c628-104">When an instance of an application from the Azure AD application gallery is added, [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) objects are created in the directory.</span></span> <span data-ttu-id="1c628-105">**ApplicationServicePrincipal**表示**应用程序**和**servicePrincipal**对象的串联。</span><span class="sxs-lookup"><span data-stu-id="1c628-105">The **applicationServicePrincipal** represents the concatenation of the **application** and **servicePrincipal** object.</span></span>

## <a name="methods"></a><span data-ttu-id="1c628-106">方法</span><span class="sxs-lookup"><span data-stu-id="1c628-106">Methods</span></span>

<span data-ttu-id="1c628-107">无</span><span class="sxs-lookup"><span data-stu-id="1c628-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="1c628-108">属性</span><span class="sxs-lookup"><span data-stu-id="1c628-108">Properties</span></span>

| <span data-ttu-id="1c628-109">属性</span><span class="sxs-lookup"><span data-stu-id="1c628-109">Property</span></span> | <span data-ttu-id="1c628-110">类型</span><span class="sxs-lookup"><span data-stu-id="1c628-110">Type</span></span>        | <span data-ttu-id="1c628-111">说明</span><span class="sxs-lookup"><span data-stu-id="1c628-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1c628-112">application</span><span class="sxs-lookup"><span data-stu-id="1c628-112">application</span></span>|[<span data-ttu-id="1c628-113">application</span><span class="sxs-lookup"><span data-stu-id="1c628-113">application</span></span>](../resources/application.md)|<span data-ttu-id="1c628-114">表示在 Azure Active Directory 中注册的应用程序。</span><span class="sxs-lookup"><span data-stu-id="1c628-114">Represents an application registered in Azure Active Directory.</span></span>|
|<span data-ttu-id="1c628-115">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="1c628-115">servicePrincipal</span></span>|[<span data-ttu-id="1c628-116">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="1c628-116">servicePrincipal</span></span>](../resources/serviceprincipal.md)|<span data-ttu-id="1c628-117">表示目录中的一个应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="1c628-117">Represents an instance of an application in a directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c628-118">关系</span><span class="sxs-lookup"><span data-stu-id="1c628-118">Relationships</span></span>

<span data-ttu-id="1c628-119">无</span><span class="sxs-lookup"><span data-stu-id="1c628-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c628-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c628-120">JSON representation</span></span>

<span data-ttu-id="1c628-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c628-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationServicePrincipal",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
   "servicePrincipal": {"@odata.type":"microsoft.graph.servicePrincipal"},
   "application": {"@odata.type":"microsoft.graph.application"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
