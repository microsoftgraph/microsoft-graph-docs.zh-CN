<!-- markdownlint-disable MD002 MD025 MD041 -->

<span data-ttu-id="52bce-101">创建垂直搜索和结果类型以自定义 必应 中的 Microsoft SharePoint、Microsoft Office 和 Microsoft 搜索中的搜索结果，以便用户更轻松地找到他们有权查看的信息。</span><span class="sxs-lookup"><span data-stu-id="52bce-101">Create search verticals and result types to customize the search results in Microsoft SharePoint, Microsoft Office, and Microsoft Search in Bing, to make it easier for users to find the information that they have permission to see.</span></span>

## <a name="create-a-vertical"></a><span data-ttu-id="52bce-102">创建垂直</span><span class="sxs-lookup"><span data-stu-id="52bce-102">Create a vertical</span></span>

<span data-ttu-id="52bce-103">若要在组织级别创建和启用垂直搜索，请Microsoft 365管理中心，全局管理员角色[](https://admin.microsoft.com/)执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="52bce-103">To create and enable a search vertical at the organization level, sign in to the [Microsoft 365 Admin center](https://admin.microsoft.com/) using the global administrator role, and do the following:</span></span>

1. <span data-ttu-id="52bce-104">转到 **"设置**  >  **搜索&**  >  **自定义"。**</span><span class="sxs-lookup"><span data-stu-id="52bce-104">Go to **Settings** > **Search & intelligence** > **Customizations**.</span></span>
2. <span data-ttu-id="52bce-105">转到 **"垂直** "，然后单击" **添加"** 按钮。</span><span class="sxs-lookup"><span data-stu-id="52bce-105">Go to **Vertical** and click the **Add** button.</span></span>
3. <span data-ttu-id="52bce-106">提供以下详细信息：</span><span class="sxs-lookup"><span data-stu-id="52bce-106">Provide the following details:</span></span>
  * <span data-ttu-id="52bce-107">**将垂直名称：** 设备部件。</span><span class="sxs-lookup"><span data-stu-id="52bce-107">**Name the vertical:** Appliance Parts.</span></span>

   !["命名垂直"部分屏幕截图](images/connectors-images/build11.png)

  * <span data-ttu-id="52bce-109">**内容源**：使用应用创建的连接器。</span><span class="sxs-lookup"><span data-stu-id="52bce-109">**Content source**: The connector created with the app.</span></span> <span data-ttu-id="52bce-110"> (部件清单) </span><span class="sxs-lookup"><span data-stu-id="52bce-110">(Parts Inventory)</span></span>

   !["内容源"部分屏幕截图](images/connectors-images/build12.png)

  * <span data-ttu-id="52bce-112">**添加查询：** 保留为空。</span><span class="sxs-lookup"><span data-stu-id="52bce-112">**Add a query**: Leave blank.</span></span>

   !["添加查询"部分屏幕截图](images/connectors-images/build13.png)

  * <span data-ttu-id="52bce-114">**筛选器**：保留为空。</span><span class="sxs-lookup"><span data-stu-id="52bce-114">**Filters**: Leave blank.</span></span>

   !["筛选器"部分屏幕截图](images/connectors-images/build14.png)

## <a name="create-a-result-type"></a><span data-ttu-id="52bce-116">创建结果类型</span><span class="sxs-lookup"><span data-stu-id="52bce-116">Create a result type</span></span>

<span data-ttu-id="52bce-117">创建结果类型：</span><span class="sxs-lookup"><span data-stu-id="52bce-117">To create a result type:</span></span>

1. <span data-ttu-id="52bce-118">转到 **"设置**  >  **搜索&**  >  **自定义"。**</span><span class="sxs-lookup"><span data-stu-id="52bce-118">Go to **Settings** > **Search & intelligence** > **Customizations**.</span></span>
2. <span data-ttu-id="52bce-119">转到结果 **类型选项卡，** 然后单击"添加 **"** 按钮。</span><span class="sxs-lookup"><span data-stu-id="52bce-119">Go to the **result type** tab and click the **Add** button.</span></span>
3. <span data-ttu-id="52bce-120">提供以下详细信息：</span><span class="sxs-lookup"><span data-stu-id="52bce-120">Provide the following details:</span></span>

  * <span data-ttu-id="52bce-121">**名称**：设备部件</span><span class="sxs-lookup"><span data-stu-id="52bce-121">**Name**: Appliance Part</span></span>

   !["命名结果类型"部分屏幕截图](images/connectors-images/build15.png)

  * <span data-ttu-id="52bce-123">**内容源**：在应用中创建的连接器。</span><span class="sxs-lookup"><span data-stu-id="52bce-123">**Content source**: The connector created in the app.</span></span>

   !["选择内容源"部分屏幕截图](images/connectors-images/build16.png)

  * <span data-ttu-id="52bce-125">**规则**：无</span><span class="sxs-lookup"><span data-stu-id="52bce-125">**Rules**: None</span></span>

   !["设置规则"部分屏幕截图](images/connectors-images/build17.png)

  * <span data-ttu-id="52bce-127">将 [ 上result-type.js粘贴](https://github.com/microsoftgraph/msgraph-search-connector-sample/blob/master/result-type.json) 到布局设计器文本框中。</span><span class="sxs-lookup"><span data-stu-id="52bce-127">Paste contents of [result-type.json](https://github.com/microsoftgraph/msgraph-search-connector-sample/blob/master/result-type.json) into the layout designer textbox.</span></span>

   !["设计布局"部分屏幕截图](images/connectors-images/build18.png)
