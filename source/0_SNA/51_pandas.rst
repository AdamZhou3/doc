^^^^^^^^^^^^
Pandas
^^^^^^^^^^^^
https://github.com/firmai/pandasvault#table-processing

Genertate DF
******************

Create Data Frame
====================
.. code-block:: python
    :linenos: 

    np.random.seed(1)
    """quick way to create a data frame for testing""" 
    df_test = pd.DataFrame(np.random.randn(3, 4), columns=['a', 'b', 'c', 'd']) \
        .assign(target=lambda x: (x['b']+x['a']/x['d'])*x['c'])
