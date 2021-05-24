---
title: userFlowLanguagePage 资源类型
description: 使用用户流语言页面可确定用户在使用用户流配置的用户旅程期间将显示的字符串。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7a52d1dce81bc24809d788e8d28ef869b84c4704
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629516"
---
# <a name="userflowlanguagepage-resource-type"></a><span data-ttu-id="822d1-103">userFlowLanguagePage 资源类型</span><span class="sxs-lookup"><span data-stu-id="822d1-103">userFlowLanguagePage resource type</span></span>

<span data-ttu-id="822d1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="822d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="822d1-105">使用用户流语言页面可确定用户在使用用户流配置的用户旅程期间将显示的字符串。</span><span class="sxs-lookup"><span data-stu-id="822d1-105">User flow language pages are used determine the strings users will be shown during the user journey you have configured using user flows.</span></span> <span data-ttu-id="822d1-106">这些语言页面包括 Microsoft 提供的默认语言翻译或可创建用于自定义语言翻译的自定义页面。</span><span class="sxs-lookup"><span data-stu-id="822d1-106">These language pages include both the default language translations provided by Microsoft, or custom pages that can be created to customize the language translations.</span></span>

## <a name="methods"></a><span data-ttu-id="822d1-107">Methods</span><span class="sxs-lookup"><span data-stu-id="822d1-107">Methods</span></span>

|<span data-ttu-id="822d1-108">方法</span><span class="sxs-lookup"><span data-stu-id="822d1-108">Method</span></span>|<span data-ttu-id="822d1-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="822d1-109">Return type</span></span>|<span data-ttu-id="822d1-110">说明</span><span class="sxs-lookup"><span data-stu-id="822d1-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="822d1-111">获取 userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="822d1-111">Get userFlowLanguagePage</span></span>](../api/userflowlanguagepage-get.md)|[<span data-ttu-id="822d1-112">userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="822d1-112">userFlowLanguagePage</span></span>](../resources/userflowlanguagepage.md)|<span data-ttu-id="822d1-113">检索默认或自定义 [userFlowLanguagePage 对象](../resources/userflowlanguagepage.md) 的值。</span><span class="sxs-lookup"><span data-stu-id="822d1-113">Retrieve the values of a default or custom [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span>|
|[<span data-ttu-id="822d1-114">更新 userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="822d1-114">Update userFlowLanguagePage</span></span>](../api/userflowlanguagepage-put.md)|[<span data-ttu-id="822d1-115">userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="822d1-115">userFlowLanguagePage</span></span>](../resources/userflowlanguagepage.md)|<span data-ttu-id="822d1-116">更新自定义 [userFlowLanguagePage 对象中的](../resources/userflowlanguagepage.md) 值。</span><span class="sxs-lookup"><span data-stu-id="822d1-116">Update the values in a custom [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span>|
|[<span data-ttu-id="822d1-117">删除 userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="822d1-117">Delete userFlowLanguagePage</span></span>](../api/userflowlanguagepage-delete.md)|<span data-ttu-id="822d1-118">无</span><span class="sxs-lookup"><span data-stu-id="822d1-118">None</span></span>|<span data-ttu-id="822d1-119">从自定义 [userFlowLanguagePage](../resources/userflowlanguagepage.md) 对象中删除值。</span><span class="sxs-lookup"><span data-stu-id="822d1-119">Deletes the values from a custom [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="822d1-120">属性</span><span class="sxs-lookup"><span data-stu-id="822d1-120">Properties</span></span>

|<span data-ttu-id="822d1-121">属性</span><span class="sxs-lookup"><span data-stu-id="822d1-121">Property</span></span>|<span data-ttu-id="822d1-122">类型</span><span class="sxs-lookup"><span data-stu-id="822d1-122">Type</span></span>|<span data-ttu-id="822d1-123">说明</span><span class="sxs-lookup"><span data-stu-id="822d1-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="822d1-124">id</span><span class="sxs-lookup"><span data-stu-id="822d1-124">id</span></span>|<span data-ttu-id="822d1-125">String</span><span class="sxs-lookup"><span data-stu-id="822d1-125">String</span></span>|<span data-ttu-id="822d1-126">userFlowLanguage 页面的标识符。</span><span class="sxs-lookup"><span data-stu-id="822d1-126">The identifier of the userFlowLanguage page.</span></span>|

## <a name="relationships"></a><span data-ttu-id="822d1-127">关系</span><span class="sxs-lookup"><span data-stu-id="822d1-127">Relationships</span></span>

<span data-ttu-id="822d1-128">无。</span><span class="sxs-lookup"><span data-stu-id="822d1-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="822d1-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="822d1-129">JSON representation</span></span>

<span data-ttu-id="822d1-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="822d1-130">The following is a JSON representation of the resource.</span></span>
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
