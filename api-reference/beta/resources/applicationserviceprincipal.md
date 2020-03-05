---
title: applicationServicePrincipal 资源类型
description: 应用程序和 servicePrincipal 的组合。
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9a7cc33e05c28e5552815778e86e5b1b9e7aaf06
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508280"
---
# <a name="applicationserviceprincipal-resource-type"></a><span data-ttu-id="67a6a-103">applicationServicePrincipal 资源类型</span><span class="sxs-lookup"><span data-stu-id="67a6a-103">applicationServicePrincipal resource type</span></span>

<span data-ttu-id="67a6a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="67a6a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67a6a-105">当添加了 Azure AD 应用程序库中的应用程序实例时，将在目录中创建[application](../resources/application.md)和[servicePrincipal](../resources/serviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="67a6a-105">When an instance of an application from the Azure AD application gallery is added, [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) objects are created in the directory.</span></span> <span data-ttu-id="67a6a-106">**ApplicationServicePrincipal**表示**应用程序**和**servicePrincipal**对象的串联。</span><span class="sxs-lookup"><span data-stu-id="67a6a-106">The **applicationServicePrincipal** represents the concatenation of the **application** and **servicePrincipal** object.</span></span>

## <a name="methods"></a><span data-ttu-id="67a6a-107">方法</span><span class="sxs-lookup"><span data-stu-id="67a6a-107">Methods</span></span>

<span data-ttu-id="67a6a-108">无</span><span class="sxs-lookup"><span data-stu-id="67a6a-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="67a6a-109">属性</span><span class="sxs-lookup"><span data-stu-id="67a6a-109">Properties</span></span>

| <span data-ttu-id="67a6a-110">属性</span><span class="sxs-lookup"><span data-stu-id="67a6a-110">Property</span></span> | <span data-ttu-id="67a6a-111">类型</span><span class="sxs-lookup"><span data-stu-id="67a6a-111">Type</span></span>        | <span data-ttu-id="67a6a-112">说明</span><span class="sxs-lookup"><span data-stu-id="67a6a-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="67a6a-113">application</span><span class="sxs-lookup"><span data-stu-id="67a6a-113">application</span></span>|[<span data-ttu-id="67a6a-114">application</span><span class="sxs-lookup"><span data-stu-id="67a6a-114">application</span></span>](../resources/application.md)|<span data-ttu-id="67a6a-115">表示在 Azure Active Directory 中注册的应用程序。</span><span class="sxs-lookup"><span data-stu-id="67a6a-115">Represents an application registered in Azure Active Directory.</span></span>|
|<span data-ttu-id="67a6a-116">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="67a6a-116">servicePrincipal</span></span>|[<span data-ttu-id="67a6a-117">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="67a6a-117">servicePrincipal</span></span>](../resources/serviceprincipal.md)|<span data-ttu-id="67a6a-118">表示目录中的一个应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="67a6a-118">Represents an instance of an application in a directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67a6a-119">关系</span><span class="sxs-lookup"><span data-stu-id="67a6a-119">Relationships</span></span>

<span data-ttu-id="67a6a-120">无</span><span class="sxs-lookup"><span data-stu-id="67a6a-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="67a6a-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="67a6a-121">JSON representation</span></span>

<span data-ttu-id="67a6a-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67a6a-122">The following is a JSON representation of the resource.</span></span>

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
