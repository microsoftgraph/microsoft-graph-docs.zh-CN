---
title: 使用连接器 API
description: Microsoft Graph 连接器 API 概述
author: mecampos
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 63e11b086592a46a4e519a2ab7c79c20d049213a
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645902"
---
# <a name="working-with-the-connectors-api"></a><span data-ttu-id="e6905-103">使用连接器 API</span><span class="sxs-lookup"><span data-stu-id="e6905-103">Working with the connectors API</span></span>

<span data-ttu-id="e6905-104">Microsoft Graph 连接器平台提供了一种简单的方法，可将外部数据添加到 Microsoft Graph 中并提升 Microsoft 365 智能体验。</span><span class="sxs-lookup"><span data-stu-id="e6905-104">Microsoft Graph connectors offer a simple way to bring external data into Microsoft Graph and enhance Microsoft 365 intelligent experiences.</span></span> <span data-ttu-id="e6905-105">你可能希望构建自定义连接器，以与未作为 Microsoft 构建的连接器的服务集成。</span><span class="sxs-lookup"><span data-stu-id="e6905-105">You might want to build a custom connector to integrate with services that aren't available as connectors built by Microsoft.</span></span> <span data-ttu-id="e6905-106">若要构建自定义连接器，请使用 Microsoft Graph 连接器 REST API。</span><span class="sxs-lookup"><span data-stu-id="e6905-106">To build custom connectors, you use the Microsoft Graph connector REST APIs.</span></span>

![图像显示外部数据即将通过不同类型的连接线连接到 Microsoft Graph](./images/connectors-images/api-overview.png)

<span data-ttu-id="e6905-108">可以使用 Microsoft Graph 连接器 API 来：</span><span class="sxs-lookup"><span data-stu-id="e6905-108">You can use the Microsoft Graph connectors API to:</span></span>

1. <span data-ttu-id="e6905-109">创建和管理外部数据连接。</span><span class="sxs-lookup"><span data-stu-id="e6905-109">Create and manage external data connections.</span></span>
2. <span data-ttu-id="e6905-110">定义和注册外部数据类型的架构。</span><span class="sxs-lookup"><span data-stu-id="e6905-110">Define and register the schema of the external data type(s).</span></span>
3. <span data-ttu-id="e6905-111">将外部数据项提取到 Microsoft Graph 中。</span><span class="sxs-lookup"><span data-stu-id="e6905-111">Ingest external data items into Microsoft Graph.</span></span>
4. <span data-ttu-id="e6905-112">同步外部组。</span><span class="sxs-lookup"><span data-stu-id="e6905-112">Sync external groups.</span></span>

<span data-ttu-id="e6905-113">如果要了解有关这些 API 的更多详细信息，可以访问下面建议的文档。</span><span class="sxs-lookup"><span data-stu-id="e6905-113">To learn more details about these APIs, you can visit the documentation suggested next.</span></span>

## <a name="connections-api"></a><span data-ttu-id="e6905-114">连接 API</span><span class="sxs-lookup"><span data-stu-id="e6905-114">Connections API</span></span>

<span data-ttu-id="e6905-115">连接是外部数据的逻辑容器，您可以作为一个单元进行管理。</span><span class="sxs-lookup"><span data-stu-id="e6905-115">A connection is a logical container for your external data that you can manage as a single unit.</span></span>
<span data-ttu-id="e6905-116">如果要了解有关如何在 Microsoft Graph 中创建、更新和删除连接的更多信息，请访问[管理连接](connecting-external-content-manage-connections.md)部分。</span><span class="sxs-lookup"><span data-stu-id="e6905-116">To learn more about how to create, update, and delete connections in the Microsoft Graph, visit the [Manage connection](connecting-external-content-manage-connections.md) section.</span></span>

## <a name="schema-api"></a><span data-ttu-id="e6905-117">架构 API</span><span class="sxs-lookup"><span data-stu-id="e6905-117">Schema API</span></span>

<span data-ttu-id="e6905-118">连接[架构](/graph/api/resources/schema?view=graph-rest-beta&amp;preserve-view=true)确定各种 Microsoft 365 体验中如何使用你的内容。</span><span class="sxs-lookup"><span data-stu-id="e6905-118">The connection [schema](/graph/api/resources/schema?view=graph-rest-beta&amp;preserve-view=true) determines how your content will be used in various Microsoft 365 experiences.</span></span> <span data-ttu-id="e6905-119">架构是计划添加到连接中的所有属性的简单列表及其属性、标签和别名。</span><span class="sxs-lookup"><span data-stu-id="e6905-119">Schema is a flat list of all the properties you plan to add to the connection along with their attributes, labels, and aliases.</span></span> <span data-ttu-id="e6905-120">必须先注册架构，然后才能将项目提取到 Microsoft Graph 中。</span><span class="sxs-lookup"><span data-stu-id="e6905-120">You must register the schema before ingesting items into Microsoft Graph.</span></span>

<span data-ttu-id="e6905-121">如果要了解有关如何为 Microsoft Graph 连接注册架构及其属性的更多信息，请访问[管理架构](connecting-external-content-manage-schema.md)部分。</span><span class="sxs-lookup"><span data-stu-id="e6905-121">To learn more about how to register the schema for the Microsoft Graph connection, and its properties, visit the [Manage schema](connecting-external-content-manage-schema.md) section.</span></span>

## <a name="ingest-external-data-items"></a><span data-ttu-id="e6905-122">提取外部数据项</span><span class="sxs-lookup"><span data-stu-id="e6905-122">Ingest external data items</span></span>

<span data-ttu-id="e6905-123">Microsoft Graph 连接器平台提供了一种简单的方法，可将外部数据添加到 Microsoft Graph 中。</span><span class="sxs-lookup"><span data-stu-id="e6905-123">Microsoft Graph connectors offer a simple way to bring external data into Microsoft Graph.</span></span> <span data-ttu-id="e6905-124">应用程序添加到 Microsoft 搜索服务的项用 Microsoft Graph 中的 [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) 资源表示。</span><span class="sxs-lookup"><span data-stu-id="e6905-124">Items added by your application to the Microsoft Search service are represented by the [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) resource in Microsoft Graph.</span></span>

<span data-ttu-id="e6905-125">如果要了解有关如何创建、更新和删除应用程序通过 Microsoft Graph 连接器添加的项目的更多信息，请访问[管理项目](connecting-external-content-manage-items.md)部分。</span><span class="sxs-lookup"><span data-stu-id="e6905-125">To learn more about how to create, update, and delete items added by your application via Microsoft Graph connectors, visit the [Manage items](connecting-external-content-manage-items.md) section.</span></span>

## <a name="external-groups-api"></a><span data-ttu-id="e6905-126">外部组 API</span><span class="sxs-lookup"><span data-stu-id="e6905-126">External groups API</span></span>

<span data-ttu-id="e6905-127">可通过 ACL 对不同类型的非 Azure Active Directory 组授予或拒绝对外部服务中的项目的访问。</span><span class="sxs-lookup"><span data-stu-id="e6905-127">Items in the external service can be granted or denied access via ACL to different types of non-Azure Active Directory groups.</span></span> <span data-ttu-id="e6905-128">例如，Salesforce 项可能拥有权限集和配置文件。</span><span class="sxs-lookup"><span data-stu-id="e6905-128">For example, Salesforce items might have permission sets and profiles.</span></span> <span data-ttu-id="e6905-129">ServiceNow 项目可能有本地组。</span><span class="sxs-lookup"><span data-stu-id="e6905-129">ServiceNow items might have local groups.</span></span> <span data-ttu-id="e6905-130">将这些项目提取到 Microsoft Graph 中时，需要遵守这些 ACL。</span><span class="sxs-lookup"><span data-stu-id="e6905-130">When you ingest these items into Microsoft Graph, you need to honor these ACLs.</span></span>

<span data-ttu-id="e6905-131">可以使用外部组 API 来设置对提取到 Microsoft Graph 中的外部项目权限。</span><span class="sxs-lookup"><span data-stu-id="e6905-131">You can use the External groups API to set permissions on external items ingested into Microsoft Graph.</span></span> <span data-ttu-id="e6905-132">[externalGroup](/graph/api/externalgroup-post-members?view=graph-rest-beta&amp;preserve-view=true) 表示非 Azure Active Directory 组或类似组的构造（例如业务部门、团队等），并确定对外部数据源中内容的权限。</span><span class="sxs-lookup"><span data-stu-id="e6905-132">An [externalGroup](/graph/api/externalgroup-post-members?view=graph-rest-beta&amp;preserve-view=true) represents a non-Azure Active Directory group or group-like construct (such as Business units, Teams, and so on) and determines permissions on the content in your external data source.</span></span>