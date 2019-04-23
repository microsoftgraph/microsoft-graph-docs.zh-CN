---
title: 使用 Microsoft Graph 将数据写入 Excel 工作簿
description: q=excelstarter)。
localization_priority: Priority
author: lumine2008
ms.prod: excel
ms.openlocfilehash: a8fcc90d4050cb6f0db2fb5e2b3a22d267f8cede
ms.sourcegitcommit: bbe42a15dad4ffe037a6934ab6001b585b7574c2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2019
ms.locfileid: "31904068"
---
# <a name="write-data-to-an-excel-workbook-with-microsoft-graph"></a><span data-ttu-id="9b138-103">使用 Microsoft Graph 将数据写入 Excel 工作簿</span><span class="sxs-lookup"><span data-stu-id="9b138-103">Write data to an Excel workbook with Microsoft Graph</span></span>

<span data-ttu-id="9b138-104">Excel REST API 提供了一种简单的、独立于平台的方法将信息上传到 Excel 工作簿。</span><span class="sxs-lookup"><span data-stu-id="9b138-104">The Excel REST API provides an easy, platform-agnostic way to upload information to an Excel workbook.</span></span> <span data-ttu-id="9b138-105">本主题介绍如何在三个 Web 开发框架上将简单数据集写入 Excel 工作簿：ASP.NET、Angular 和 React。</span><span class="sxs-lookup"><span data-stu-id="9b138-105">This topic shows you how to write simple data sets to an Excel workbook on three web development frameworks: ASP.NET, Angular, and React.</span></span> <span data-ttu-id="9b138-106">你可以通过访问 [GitHub 上的 Microsoft Graph Excel 入门版示例](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=excelstarter)来查看本主题所采用的代码示例。</span><span class="sxs-lookup"><span data-stu-id="9b138-106">You can look at the code samples featured in this topic by visiting the [Microsoft Graph Excel starter samples on GitHub](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=excelstarter).</span></span>

> <span data-ttu-id="9b138-107">**注意：** 这三个示例将数据写入名为 **demo.xlsx** 的 Excel 工作簿。</span><span class="sxs-lookup"><span data-stu-id="9b138-107">**Note:** All three of the samples write data to an Excel workbook named **demo.xlxs**.</span></span> <span data-ttu-id="9b138-108">它们都提供了此工作簿，以便你可以将其上传到你自己的 OneDrive，不过，你也可以使用 Microsoft Graph 将文件上传到 OneDrive。</span><span class="sxs-lookup"><span data-stu-id="9b138-108">They provide this workbook for you so that you can upload it to your own OneDrive, but you can also use Microsoft Graph to upload files to OneDrive.</span></span> <span data-ttu-id="9b138-109">如果有意了解 REST 调用，你需要将任何类型的文件上传到你的 OneDrive 根文件夹，请参阅 [Microsoft Graph Excel REST API ASP.NET 待办事项列表示例](https://github.com/microsoftgraph/aspnet-todo-rest-sample)。</span><span class="sxs-lookup"><span data-stu-id="9b138-109">If you're interested in learning the REST calls you need to upload a file of any type to your root OneDrive folder, see the [Microsoft Graph Excel REST API ASP.NET to-do list sample](https://github.com/microsoftgraph/aspnet-todo-rest-sample).</span></span>

<span data-ttu-id="9b138-110">这三个 Excel 入门版示例均执行相同的操作：检索登录用户的名称和地址，并将这两条信息添加到 demo.xlsx\*\*\*\* 工作簿中的新行。</span><span class="sxs-lookup"><span data-stu-id="9b138-110">All three of the Excel starter samples do the same thing: retrieve the name and address of the signed-in user and add those two pieces of information to a new row in the **demo.xlsx** workbook.</span></span> <span data-ttu-id="9b138-111">你可以通过将信息添加到代表你想要添加的一行或多行的二维数组中来修改示例，以添加额外的行。</span><span class="sxs-lookup"><span data-stu-id="9b138-111">You can modify the samples to add additional rows simply by adding information to the two-dimensional array that represents the row or rows that you want to add.</span></span>

## <a name="add-a-row-or-rows-to-an-excel-workbook-with-a-single-rest-request"></a><span data-ttu-id="9b138-112">使用单个 REST 请求将一行或多行添加到 Excel 工作簿</span><span class="sxs-lookup"><span data-stu-id="9b138-112">Add a row or rows to an Excel workbook with a single REST request</span></span>

<span data-ttu-id="9b138-113">Excel REST API 要求将简单的请求正文发布到代表 Excel 工作簿行集合的 REST 终结点。</span><span class="sxs-lookup"><span data-stu-id="9b138-113">The Excel REST API requires you to POST a simple request body to the REST endpoint that represents the row collection of an Excel workbook.</span></span> <span data-ttu-id="9b138-114">如果你正在使用登录用户 OneDrive 帐户根文件夹中的笔记本，REST 终结点将如下所示：</span><span class="sxs-lookup"><span data-stu-id="9b138-114">If you're working with a notebook in the root folder of the signed-in user's OneDrive account, the REST endpoint will look like this:</span></span>

`https://graph.microsoft.com/v1.0/me/drive/root:/demo.xlsx:/workbook/tables/Table1/rows/add`

<span data-ttu-id="9b138-115">有关如何获取 OneDrive 文件夹中文件的详细信息，请参阅我们参考文档中的 [DriveItem 资源类型](/graph/api/resources/driveitem?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="9b138-115">For more information about how to reach files in OneDrive folders, see the [DriveItem resource type](/graph/api/resources/driveitem?view=graph-rest-1.0) in our reference documentation.</span></span>

> <span data-ttu-id="9b138-116">**注意：** 可以通过将 GET 请求发送到以 `/rows` 结尾的路径部分来查看工作簿的现有行集合。</span><span class="sxs-lookup"><span data-stu-id="9b138-116">**Note:** You can look at the existing row collection of the workbook by making a GET request to the part of the path that ends at `/rows`.</span></span>

<span data-ttu-id="9b138-117">POST 正文如下所示：</span><span class="sxs-lookup"><span data-stu-id="9b138-117">The POST body looks like this:</span></span>

`{
  "index": null,
  "values": [
    ['alex darrow', 'adarrow@tenant.onmicrosoft.com']
  ]
}`

<span data-ttu-id="9b138-118">第一个 `index` 参数的值指定要添加到零索引行数组的行的相对位置。</span><span class="sxs-lookup"><span data-stu-id="9b138-118">The value of the first `index` parameter specifies the relative position of the row that you're adding to the zero-indexed array of rows.</span></span> <span data-ttu-id="9b138-119">插入行下方的行将会向下移动。</span><span class="sxs-lookup"><span data-stu-id="9b138-119">Rows below the inserted row will be shifted downwards.</span></span> <span data-ttu-id="9b138-120">`null` 参数指示将添加到结尾的新行。</span><span class="sxs-lookup"><span data-stu-id="9b138-120">The `null` parameter indicates that the new row will be added to the end.</span></span>

<span data-ttu-id="9b138-121">第二个 `values` 参数的值是一个二维字符串数组，其中包含要添加的每一行未格式化的值。</span><span class="sxs-lookup"><span data-stu-id="9b138-121">The value of the second `values` parameter is a two-dimensional string array that contains the unformatted values of each row that you want to add.</span></span> <span data-ttu-id="9b138-122">示例中的数组仅包含一行，但可以通过添加更多字符串数组添加更多行。</span><span class="sxs-lookup"><span data-stu-id="9b138-122">The array in the sample contains only one row, but you can add more rows by adding more string arrays.</span></span>

<span data-ttu-id="9b138-123">通过将 demo.xlsx 文件上传到 OneDrive 根文件夹并在 [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) 上执行此查询，便可使用你自己的 OneDrive 帐户测试此查询。</span><span class="sxs-lookup"><span data-stu-id="9b138-123">You can test this query with your own OneDrive account by uploading the demo.xlsx file to your OneDrive root folder and executing this query on the [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

<span data-ttu-id="9b138-124">这是将数据写入 Excel 工作簿所需了解的全部内容。</span><span class="sxs-lookup"><span data-stu-id="9b138-124">That is all you need to know in order to write data to an Excel workbook.</span></span> <span data-ttu-id="9b138-125">你需要了解如何在你自己框架中构造并发出请求，Excel 入门版示例演示了执行此操作的三种不同方式。</span><span class="sxs-lookup"><span data-stu-id="9b138-125">You do need to know how to construct and make the request in your own framework, and the Excel starter samples demonstrate three separate ways of doing this.</span></span>

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-aspnet"></a><span data-ttu-id="9b138-126">将一行或多行添加到 ASP.NET Excel 工作簿</span><span class="sxs-lookup"><span data-stu-id="9b138-126">Add a row or rows to an Excel workbook in ASP.NET</span></span>

<span data-ttu-id="9b138-127">你可以在 [ASP.NET 4.6 Microsoft Graph Excel 入门版示例](https://github.com/microsoftgraph/aspnet-excelstarter-sample)的 [GraphResources.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphResources.cs) 和 [GraphService.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphService.cs) 文件中找到构造和发送请求的 ASP.NET 代码。</span><span class="sxs-lookup"><span data-stu-id="9b138-127">You'll find the ASP.NET code that constructs and sends the request in the [GraphResources.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphResources.cs) and [GraphService.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphService.cs) files of the [Microsoft Graph Excel Starter Sample for ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-excelstarter-sample).</span></span>

<span data-ttu-id="9b138-128">`GraphResources.cs` 文件提供了帮助程序类，用于封装从 Microsoft Graph 中检索的用户数据，以及在写入工作簿时将使用的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9b138-128">The `GraphResources.cs` file provides a helper class for encapsulating both the user data you're retrieving from Microsoft Graph and the request body that you'll use when you write to your workbook.</span></span>

    public class UserInfo
    {
        public string Name { get; set; }
        public string Address { get; set; }

    }

    public class UserInfoRequest
    {
        public string index { get; set; }
        public string[][] values { get; set; }
    }

<span data-ttu-id="9b138-129">`GraphService.cs` 类包含 `AddInfoToExcel` 方法，可用于填充这些类、将请求信息序列化为 JSON 对象，然后将该对象作为 POST 请求正文传递。</span><span class="sxs-lookup"><span data-stu-id="9b138-129">The `GraphService.cs` class contains an `AddInfoToExcel` method that populates these classes, serializes the request information into a JSON object, and then passes that object as the POST request body.</span></span>

        public async Task<string> AddInfoToExcel(string accessToken, string name, string address)
        {
            string endpoint = "https://graph.microsoft.com/v1.0/me/drive/root:/demo.xlsx:/workbook/tables/Table1/rows/add";
            using (var client = new HttpClient())
            {
                using (var request = new HttpRequestMessage(HttpMethod.Post, endpoint))
                {
                    // Populate UserInfoRequest object
                    string[] userInfo = { name, address  };
                    string[][] userInfoArray = { userInfo };
                    UserInfoRequest userInfoRequest = new UserInfoRequest();
                    userInfoRequest.index = null;
                    userInfoRequest.values = userInfoArray;

                    // Serialize the information in the UserInfoRequest object
                    string jsonBody = JsonConvert.SerializeObject(userInfoRequest);
                    request.Headers.Accept.Add(new MediaTypeWithQualityHeaderValue("application/json"));
                    request.Headers.Authorization = new AuthenticationHeaderValue("Bearer", accessToken);
                    request.Content = new StringContent(jsonBody, Encoding.UTF8, "application/json");

                    using (var response = await client.SendAsync(request))
                    {
                        if (response.IsSuccessStatusCode)
                        {
                            return Resource.Graph_UploadToExcel_Success_Result;
                        }
                        return response.ReasonPhrase;
                    }
                }
            }
        }

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-angular"></a><span data-ttu-id="9b138-130">将一行或多行添加到 Angular Excel 工作簿</span><span class="sxs-lookup"><span data-stu-id="9b138-130">Add a row or rows to an Excel workbook in Angular</span></span>

<span data-ttu-id="9b138-131">你可以在 [Angular Microsoft Graph Excel 入门版示例](https://github.com/microsoftgraph/angular-excelstarter-sample)的 [home.service.ts 文件](https://github.com/microsoftgraph/angular-excelstarter-sample/blob/master/src/app/home/home.service.ts)中找到构造和发送请求的 Angular 代码。</span><span class="sxs-lookup"><span data-stu-id="9b138-131">You'll find the Angular code that constructs and sends the request in the [home.service.ts file](https://github.com/microsoftgraph/angular-excelstarter-sample/blob/master/src/app/home/home.service.ts) of the [Microsoft Graph Excel Starter Sample for Angular](https://github.com/microsoftgraph/angular-excelstarter-sample).</span></span>

<span data-ttu-id="9b138-132">由于本示例使用 TypeScript，因此，它利用 [Microsoft Graph JavaScript 客户端库](https://github.com/microsoftgraph/msgraph-sdk-javascript)和 [Microsoft Graph TypeScript 类型](https://github.com/microsoftgraph/msgraph-typescript-typings)。</span><span class="sxs-lookup"><span data-stu-id="9b138-132">Since this sample uses TypeScript, it takes advantage of the [Microsoft Graph JavaScript Client Library](https://github.com/microsoftgraph/msgraph-sdk-javascript) and the [ Microsoft Graph TypeScript Types](https://github.com/microsoftgraph/msgraph-typescript-typings).</span></span>

<span data-ttu-id="9b138-133">`home.service.ts` 文件中的 `addInfoToExcel` 函数构造二维字符串数组和包含数组的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9b138-133">The `addInfoToExcel` function in the `home.service.ts` file constructs the two-dimensional string array and the request body that contains the array.</span></span> <span data-ttu-id="9b138-134">然后使用 Microsoft Graph JavaScript 客户端库构造和发送请求。</span><span class="sxs-lookup"><span data-stu-id="9b138-134">It then uses the Microsoft Graph JavaScript Client Library to construct and send the request.</span></span> <span data-ttu-id="9b138-135">响应以承诺的形式返回。</span><span class="sxs-lookup"><span data-stu-id="9b138-135">The response comes back in the form of a Promise.</span></span>

      addInfoToExcel(user: MicrosoftGraph.User) {
        const userInfo = [];
        const userEmail = user.mail || user.userPrincipalName;    
        userInfo.push([user.displayName, userEmail]);

        const userInfoRequestBody = {
          index: null,
          values: userInfo
        };   

        const body = JSON.stringify(userInfoRequestBody);

        var client = this.getClient();
        var url = `${this.url}/me/drive/root:/${this.file}:/workbook/tables/${this.table}/rows/add`
        return Observable.fromPromise(client
        .api(url)
        .post(body)
        );
      }

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-react"></a><span data-ttu-id="9b138-136">将一行或多行添加到 React Excel 工作簿</span><span class="sxs-lookup"><span data-stu-id="9b138-136">Add a row or rows to an Excel workbook in React</span></span>

<span data-ttu-id="9b138-137">你可以在 [React Microsoft Graph Excel 入门版示例](https://github.com/microsoftgraph/react-excelstarter-sample)的 [home.js 文件](https://github.com/microsoftgraph/react-excelstarter-sample/blob/master/src/home/home.js)中找到构造和发送请求的代码。</span><span class="sxs-lookup"><span data-stu-id="9b138-137">You'll find the code that constructs and sends the request in the [home.js file](https://github.com/microsoftgraph/react-excelstarter-sample/blob/master/src/home/home.js) of the [Microsoft Graph Excel Starter Sample for React](https://github.com/microsoftgraph/react-excelstarter-sample).</span></span>

<span data-ttu-id="9b138-138">`onWriteToExcel` 函数构造二维字符串数组并将其作为请求正文传递。</span><span class="sxs-lookup"><span data-stu-id="9b138-138">The `onWriteToExcel` function constructs the two-dimensional string array and passes it as the request body.</span></span> <span data-ttu-id="9b138-139">它使用 [axios](https://www.npmjs.com/package/axios) 发出进行 HTTP 请求。</span><span class="sxs-lookup"><span data-stu-id="9b138-139">It uses [axios](https://www.npmjs.com/package/axios) to make the HTTP request.</span></span>

      onWriteToExcel() {
        const { token, me } = this.state;

        const myEmailAddress = me.mail || me.userPrincipalName;
        const values = [];

        values.push([me.displayName, myEmailAddress]);

        axios
          .post('https://graph.microsoft.com/v1.0/me/drive/root:/demo.xlsx:/workbook/tables/Table1/rows/add',
            { index: null, values },
            { headers: { Authorization: `Bearer ${token}` }}
          )
          .then(res => {
                          console.log(res);
                          const successMessage = "Successfully wrote your data to demo.xlsx!";
                          this.setState ({ successMessage });
                         })
          .catch(err => console.error(err));
      }

##<a name="see-also"></a><span data-ttu-id="9b138-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="9b138-140">See also</span></span>

* [<span data-ttu-id="9b138-141">通过 Microsoft Graph 管理 Excel 会话</span><span class="sxs-lookup"><span data-stu-id="9b138-141">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="9b138-142">通过 Microsoft Graph 使用 Excel 工作簿函数</span><span class="sxs-lookup"><span data-stu-id="9b138-142">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="9b138-143">通过 Microsoft Graph 更新 Excel 区域的格式</span><span class="sxs-lookup"><span data-stu-id="9b138-143">Update a range’s format in Excel with Microsoft Graph</span></span>](excel-update-range-format.md)
* [<span data-ttu-id="9b138-144">通过 Microsoft Graph 显示 Excel 图表图像</span><span class="sxs-lookup"><span data-stu-id="9b138-144">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="9b138-145">使用 Excel REST API</span><span class="sxs-lookup"><span data-stu-id="9b138-145">Use the Excel REST API</span></span>](/graph/api/resources/excel?view=graph-rest-1.0)    
