---
title: userFlowLanguagePage 资源类型
description: 确定在用户流期间向用户显示的字符串。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b3f3610607bfeef5f3e47a110c2491b635555494
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882939"
---
# <a name="userflowlanguagepage-resource-type"></a><span data-ttu-id="0e3e4-103">userFlowLanguagePage 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e3e4-103">userFlowLanguagePage resource type</span></span>

<span data-ttu-id="0e3e4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e3e4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0e3e4-105">确定在用户流期间向用户显示的用户流语言页面。</span><span class="sxs-lookup"><span data-stu-id="0e3e4-105">Determines the user flow language pages that are shown to users during a user flow.</span></span> <span data-ttu-id="0e3e4-106">这些语言页面包括 Microsoft 提供的默认语言翻译或可创建用于自定义语言翻译的自定义页面。</span><span class="sxs-lookup"><span data-stu-id="0e3e4-106">These language pages include both the default language translations provided by Microsoft, or custom pages that can be created to customize the language translations.</span></span>

## <a name="methods"></a><span data-ttu-id="0e3e4-107">方法</span><span class="sxs-lookup"><span data-stu-id="0e3e4-107">Methods</span></span>

|<span data-ttu-id="0e3e4-108">方法</span><span class="sxs-lookup"><span data-stu-id="0e3e4-108">Method</span></span>|<span data-ttu-id="0e3e4-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="0e3e4-109">Return type</span></span>|<span data-ttu-id="0e3e4-110">说明</span><span class="sxs-lookup"><span data-stu-id="0e3e4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0e3e4-111">获取 userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="0e3e4-111">Get userFlowLanguagePage</span></span>](../api/userflowlanguagepage-get.md)|[<span data-ttu-id="0e3e4-112">userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="0e3e4-112">userFlowLanguagePage</span></span>](../resources/userflowlanguagepage.md)|<span data-ttu-id="0e3e4-113">检索默认或自定义 [userFlowLanguagePage 对象](../resources/userflowlanguagepage.md) 的值。</span><span class="sxs-lookup"><span data-stu-id="0e3e4-113">Retrieve the values of a default or custom [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span>|
|[<span data-ttu-id="0e3e4-114">更新 userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="0e3e4-114">Update userFlowLanguagePage</span></span>](../api/userflowlanguagepage-put.md)|[<span data-ttu-id="0e3e4-115">userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="0e3e4-115">userFlowLanguagePage</span></span>](../resources/userflowlanguagepage.md)|<span data-ttu-id="0e3e4-116">更新自定义 [userFlowLanguagePage 对象中的](../resources/userflowlanguagepage.md) 值。</span><span class="sxs-lookup"><span data-stu-id="0e3e4-116">Update the values in a custom [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span>|
|[<span data-ttu-id="0e3e4-117">删除 userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="0e3e4-117">Delete userFlowLanguagePage</span></span>](../api/userflowlanguagepage-delete.md)|<span data-ttu-id="0e3e4-118">无</span><span class="sxs-lookup"><span data-stu-id="0e3e4-118">None</span></span>|<span data-ttu-id="0e3e4-119">从自定义 [userFlowLanguagePage](../resources/userflowlanguagepage.md) 对象中删除值。</span><span class="sxs-lookup"><span data-stu-id="0e3e4-119">Deletes the values from a custom [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0e3e4-120">属性</span><span class="sxs-lookup"><span data-stu-id="0e3e4-120">Properties</span></span>

|<span data-ttu-id="0e3e4-121">属性</span><span class="sxs-lookup"><span data-stu-id="0e3e4-121">Property</span></span>|<span data-ttu-id="0e3e4-122">类型</span><span class="sxs-lookup"><span data-stu-id="0e3e4-122">Type</span></span>|<span data-ttu-id="0e3e4-123">说明</span><span class="sxs-lookup"><span data-stu-id="0e3e4-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e3e4-124">id</span><span class="sxs-lookup"><span data-stu-id="0e3e4-124">id</span></span>|<span data-ttu-id="0e3e4-125">String</span><span class="sxs-lookup"><span data-stu-id="0e3e4-125">String</span></span>|<span data-ttu-id="0e3e4-126">userFlowLanguage 页面的标识符。</span><span class="sxs-lookup"><span data-stu-id="0e3e4-126">The identifier of the userFlowLanguage page.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e3e4-127">关系</span><span class="sxs-lookup"><span data-stu-id="0e3e4-127">Relationships</span></span>

<span data-ttu-id="0e3e4-128">无。</span><span class="sxs-lookup"><span data-stu-id="0e3e4-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e3e4-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e3e4-129">JSON representation</span></span>

<span data-ttu-id="0e3e4-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e3e4-130">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userFlowLanguagePage",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userFlowLanguagePage",
  "id": "String (identifier)"
}
```
