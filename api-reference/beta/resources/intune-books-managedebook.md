---
title: managedEBook 资源类型
description: 包含托管电子书基属性的抽象类。
author: tfitzmac
ms.openlocfilehash: 7b826d7b0a11ce957a87154f276abc0e8168f45d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347143"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="4e1f1-103">managedEBook 资源类型</span><span class="sxs-lookup"><span data-stu-id="4e1f1-103">managedEBook resource type</span></span>

> <span data-ttu-id="4e1f1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4e1f1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e1f1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4e1f1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e1f1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4e1f1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e1f1-107">包含托管电子书基属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="4e1f1-107">An abstract class containing the base properties for Managed eBook.</span></span>
## <a name="methods"></a><span data-ttu-id="4e1f1-108">方法</span><span class="sxs-lookup"><span data-stu-id="4e1f1-108">Methods</span></span>
|<span data-ttu-id="4e1f1-109">方法</span><span class="sxs-lookup"><span data-stu-id="4e1f1-109">Method</span></span>|<span data-ttu-id="4e1f1-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="4e1f1-110">Return Type</span></span>|<span data-ttu-id="4e1f1-111">说明</span><span class="sxs-lookup"><span data-stu-id="4e1f1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4e1f1-112">List managedEBooks</span><span class="sxs-lookup"><span data-stu-id="4e1f1-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="4e1f1-113">[managedEBook](../resources/intune-books-managedebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4e1f1-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="4e1f1-114">列出 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4e1f1-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="4e1f1-115">Get managedEBook</span><span class="sxs-lookup"><span data-stu-id="4e1f1-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="4e1f1-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="4e1f1-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="4e1f1-117">读取 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4e1f1-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="4e1f1-118">assign 操作</span><span class="sxs-lookup"><span data-stu-id="4e1f1-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="4e1f1-119">无</span><span class="sxs-lookup"><span data-stu-id="4e1f1-119">None</span></span>|<span data-ttu-id="4e1f1-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4e1f1-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="4e1f1-121">属性</span><span class="sxs-lookup"><span data-stu-id="4e1f1-121">Properties</span></span>
|<span data-ttu-id="4e1f1-122">属性</span><span class="sxs-lookup"><span data-stu-id="4e1f1-122">Property</span></span>|<span data-ttu-id="4e1f1-123">类型</span><span class="sxs-lookup"><span data-stu-id="4e1f1-123">Type</span></span>|<span data-ttu-id="4e1f1-124">说明</span><span class="sxs-lookup"><span data-stu-id="4e1f1-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e1f1-125">id</span><span class="sxs-lookup"><span data-stu-id="4e1f1-125">id</span></span>|<span data-ttu-id="4e1f1-126">String</span><span class="sxs-lookup"><span data-stu-id="4e1f1-126">String</span></span>|<span data-ttu-id="4e1f1-127">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4e1f1-127">Key of the entity.</span></span>|
|<span data-ttu-id="4e1f1-128">displayName</span><span class="sxs-lookup"><span data-stu-id="4e1f1-128">displayName</span></span>|<span data-ttu-id="4e1f1-129">String</span><span class="sxs-lookup"><span data-stu-id="4e1f1-129">String</span></span>|<span data-ttu-id="4e1f1-130">电子书的名称。</span><span class="sxs-lookup"><span data-stu-id="4e1f1-130">Name of the eBook.</span></span>|
|<span data-ttu-id="4e1f1-131">description</span><span class="sxs-lookup"><span data-stu-id="4e1f1-131">description</span></span>|<span data-ttu-id="4e1f1-132">String</span><span class="sxs-lookup"><span data-stu-id="4e1f1-132">String</span></span>|<span data-ttu-id="4e1f1-133">说明。</span><span class="sxs-lookup"><span data-stu-id="4e1f1-133">Description.</span></span>|
|<span data-ttu-id="4e1f1-134">publisher</span><span class="sxs-lookup"><span data-stu-id="4e1f1-134">publisher</span></span>|<span data-ttu-id="4e1f1-135">String</span><span class="sxs-lookup"><span data-stu-id="4e1f1-135">String</span></span>|<span data-ttu-id="4e1f1-136">发布者。</span><span class="sxs-lookup"><span data-stu-id="4e1f1-136">Publisher.</span></span>|
|<span data-ttu-id="4e1f1-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e1f1-137">publishedDateTime</span></span>|<span data-ttu-id="4e1f1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e1f1-138">DateTimeOffset</span></span>|<span data-ttu-id="4e1f1-139">电子书的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4e1f1-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="4e1f1-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="4e1f1-140">largeCover</span></span>|[<span data-ttu-id="4e1f1-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4e1f1-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4e1f1-142">书籍封面。</span><span class="sxs-lookup"><span data-stu-id="4e1f1-142">Book cover.</span></span>|
|<span data-ttu-id="4e1f1-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4e1f1-143">createdDateTime</span></span>|<span data-ttu-id="4e1f1-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e1f1-144">DateTimeOffset</span></span>|<span data-ttu-id="4e1f1-145">电子书文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4e1f1-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="4e1f1-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e1f1-146">lastModifiedDateTime</span></span>|<span data-ttu-id="4e1f1-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e1f1-147">DateTimeOffset</span></span>|<span data-ttu-id="4e1f1-148">上次修改电子书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4e1f1-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="4e1f1-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4e1f1-149">informationUrl</span></span>|<span data-ttu-id="4e1f1-150">String</span><span class="sxs-lookup"><span data-stu-id="4e1f1-150">String</span></span>|<span data-ttu-id="4e1f1-151">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="4e1f1-151">The more information Url.</span></span>|
|<span data-ttu-id="4e1f1-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4e1f1-152">privacyInformationUrl</span></span>|<span data-ttu-id="4e1f1-153">String</span><span class="sxs-lookup"><span data-stu-id="4e1f1-153">String</span></span>|<span data-ttu-id="4e1f1-154">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="4e1f1-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e1f1-155">关系</span><span class="sxs-lookup"><span data-stu-id="4e1f1-155">Relationships</span></span>
|<span data-ttu-id="4e1f1-156">关系</span><span class="sxs-lookup"><span data-stu-id="4e1f1-156">Relationship</span></span>|<span data-ttu-id="4e1f1-157">类型</span><span class="sxs-lookup"><span data-stu-id="4e1f1-157">Type</span></span>|<span data-ttu-id="4e1f1-158">说明</span><span class="sxs-lookup"><span data-stu-id="4e1f1-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e1f1-159">categories</span><span class="sxs-lookup"><span data-stu-id="4e1f1-159">categories</span></span>|<span data-ttu-id="4e1f1-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md)集合</span><span class="sxs-lookup"><span data-stu-id="4e1f1-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="4e1f1-161">此电子图书类别列表。</span><span class="sxs-lookup"><span data-stu-id="4e1f1-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="4e1f1-162">assignments</span><span class="sxs-lookup"><span data-stu-id="4e1f1-162">assignments</span></span>|<span data-ttu-id="4e1f1-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4e1f1-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="4e1f1-164">此电子书的分配列表。</span><span class="sxs-lookup"><span data-stu-id="4e1f1-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="4e1f1-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="4e1f1-165">installSummary</span></span>|[<span data-ttu-id="4e1f1-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="4e1f1-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="4e1f1-167">移动应用安装摘要。</span><span class="sxs-lookup"><span data-stu-id="4e1f1-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="4e1f1-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="4e1f1-168">deviceStates</span></span>|<span data-ttu-id="4e1f1-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4e1f1-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="4e1f1-170">此电子书的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="4e1f1-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="4e1f1-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="4e1f1-171">userStateSummary</span></span>|<span data-ttu-id="4e1f1-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4e1f1-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="4e1f1-173">此电子书的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="4e1f1-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4e1f1-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4e1f1-174">JSON Representation</span></span>
<span data-ttu-id="4e1f1-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4e1f1-175">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```





